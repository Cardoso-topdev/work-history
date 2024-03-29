# My sites <br />
  ## React templates
   - [material-kit](https://material-kit-react-sooty.vercel.app/)   `https://material-kit-react-sooty.vercel.app`
   - [tailwind landingpage template](https://oscar-tailwind-landing.vercel.app/)    `https://oscar-tailwind-landing.vercel.app`
   - [fuse theme](https://react-fuse.vercel.app/)   `https://react-fuse.vercel.app`
  ## Angular template
   - [CoreUI Angular 2+ Admin Template](https://core-ui-angular-template.vercel.app/)  `https://core-ui-angular-template.vercel.app`
   - [Ngx-Admin Angular template](https://ngx-template.vercel.app/) `https://ngx-template.vercel.app`
  ## Bootstrap templates
   - [Volt template](https://oscar-volt-bootstrap.netlify.app/)   `https://oscar-volt-bootstrap.netlify.app/` <br />
  ## Next.js templates
   - [next.js template1](https://nextjs-template1.vercel.app/)  `https://nextjs-template1.vercel.app/` <br />
  ## Gatsby template
   - [Prismic multi-lang template](https://prismic-gatsby-template.vercel.app/)   `https://prismic-gatsby-template.vercel.app/`
  ## Jamestack git repository 
   - [git rep](https://github.com/stackbit/jamstackthemes)
   - [live site](https://jamstackthemes.dev/)
  
  [Gatsby-Prismic for SSG with headlessCMS](https://canfone-five.vercel.app/)     `https://canfone-five.vercel.app/`  <br />
  [typeW](https://typew.com/)           `https://typew.com/`  <br />
  [gohirenow](https://www.gohirenow.com/)         `https://www.gohirenow.com/` <br />
  [useChore](https://usechore.netlify.app/)           `https://usechore.netlify.app/` <br />
  [workplace landing](https://oscar-workplace-credit.netlify.app/)          `https://oscar-workplace-credit.netlify.app/` <br />
  [One net landing](https://oscar-one-net-test.netlify.app/)          `https://oscar-one-net-test.netlify.app/` <br />
  [update click](https://oscar-update-click.netlify.app/)           `https://oscar-update-click.netlify.app/`  <br />
  [next.js sayem](https://sayem-nextjs-vercel.vercel.app)         `https://sayem-nextjs-vercel.vercel.app/` <br />
  [shopify siete](https://sietefoods.com/)          `https://sietefoods.com/` <br />
  
# work-history
## 12. Calendar App
  [git rep](https://github.com/Cardoso-topdev/calendar-app) <br />
  [live site](https://securities-calendar.herokuapp.com) <br />
  ### About
    Used React.js as a front-end framework, Express/node.js as a backend framework, and MongoDB as a backend.

    Only the administrator can input/edit/delete studying material. 
    Students can schedule their diary plans according to the supported methods. 
    There are two types of schedules: select the test date automatically and manually. 
    Students can choose the days to study. 
    With an auto choosing plan, students can set hours per day. 
    After scheduled, that schedule can be saved by email.
  ### Technologies
   - React
   - Express
   - MongoDB
   - Calendar
   - Bulk mail
   - Express Cron job
## 11. peacenik
  [git rep](https://github.com/KotoLLC/peacenik)  <br />
  [live site](https://koto.at/)  <br />
  ### About
    This is an on-going project. 
    I am responsible for developing front-end(React). 
    Slack for communication tool. 
    Git for project version control and management. 
    Docker for setup environment.
  ### Technologies
  - Docker
  - React
  - Golang
  - MinIO aws s3 
  - PostgreSQL
## 10. Canfone 
  [git rep](https://github.com/Cardoso-topdev/canfone-gatsby)   <br />
  [origin site](https://www.canfone.com/) <br />
  [current site](http://canfone.surge.sh/) <br />
### Description 
  Convert static Html/css/javascript to Gatsby Site. Integrating Prismic for content writer.
  You can simply get the main work-flow/idea of Gatsby with headlessCMS(Prismic) from this [video](./assets/video/prismic-rec.webm)
### Things what I've done
  - Fixed a small issue for styling. After launch tailwind style was not applied. That was due to mis-editing purge option on tailwind-config.json file.
  - Created multi-lang page on Prismic. You can use GraphQL query for load multi-lang page content. 
  - Multi-lang implemented by using i18n package. After install i18n, you have to create files for supporting multi-lang. ex: index.fr.js : this file will be called when url is /fr/
  - Javascript window.onload() function over-writting problem solved. it doesn't works well on develop environment, but works well on product after built and deployed to surge.
  - Used Helmet for importing js library on pages. Also used withPrefix() function for loading script after document load.
  - Convert React component to gatsby components. In original version, they used React components as javascript library. 
  - Solve SSR errors. When building the project, some objects such as document and window is not allowed on server side. So the variables and functions that referenced that object make error when building. So we have to check if document or window is defined.
  - Create imgLoader service instance for load all images. Because, Gatsby as a static site generator, all assets resources directory change when it has built. So need imgLoader service.
  - Deployed on surge using surge command line. ex: `surge public\`
  - Convert static web pages to Gatsby Project.
  - Create new Gatsby project.

## 9. Prismic Gatsby 
  [Live Site](https://prismic-gatsby-template.vercel.app/)  <br />
  [git rep](https://github.com/Cardoso-topdev/prismic-gatsby-multi-template)
  
  [working site](http://canfone.surge.sh)
  
### Technologies
  - Create account on [prismic](https://prismic.io/) 
  - Create repository on prismic
  - Create document(content writer page) on repository
  - Create custom types on repository
  - Create Prismic Gatsby template project using this command
  ```
    npm install -g prismic-cli`
    prismic theme --theme-url https://github.com/prismicio/reactjs-website --conf src/prismic-configuration.js
  ```  
  - Git push 
  - Deploy on Vercel
  - Reference pages on Prismic at php framework
    [php project git rep](https://github.com/Cardoso-topdev/benjamin-proj)
    1) composer install && composer.json 
    ```
        "name": "benjamin/php_quickstart",
        "version": "2.0",
        "require": {
          "php": ">=7.1",
          "prismic/php-sdk": "^5.0.1",
          "slim/slim": "^3.10"
        }
    ```    
    2) app/app.php
    ```
        $app->get('/', function ($request, $response, $args) use ($app, $prismic) {
            // Query the API
            $api = $prismic->get_api();
            $document = $api->getByUID('page', 'first-page');

            // Render the page
            render($app, 'home', array('document' => $document));
        });
    ```
    3) app/views/home.php
    ```
        <?php
        use Prismic\Dom\RichText;

        $document = $WPGLOBAL['document'];
        ?>

        <?php include_once 'header.php'; ?>

        <div class="welcome">
            <img src="<?= $document->data->image->url ?>" class="star"/>
            <h1><?= RichText::asText($document->data->title) ?></h1>
            <div>
                <?= RichText::asHtml($document->data->description) ?>
            </div>
        </div>

        <?php include_once 'footer.php'; ?>
    ```
    4) Run php project
    ```
        sh serve.sh
    ```    

## 8. advanced-react-hook
### Overview of advanced-react-hook project.

#### Technologies
  - material-UI
  - Integrating REST full APIs by using axios
  - Test for unit test, CypressCI for e2e test
  - draftail/draft-js library for content creator
  - mobx for managing application data
  - latest react router for routes. Comfortable tree-structured routes with easy-usable authentication route.
  - Redux for managing application data
  - redux-logger middleware for redux action && state log
  - redux-saga and redux-thunk middlewares for comfortable managind redux actions and data
  - redux-persist for storing redux data to localstorage for keeping redux data
 
#### Pages
  - Crop <br />
      `Cropping image with zooming, rotating, opening image files functions`
  - Custom Hook <br />
      `Custom hooks for using useState on functional components as componentDidMount and componentDidUpdate function on class component.`
      `And some other hooks on functional components.`
  - draftail <br />
      `Content creator page.`
  - Homepage <br />
      `Simple homepage`
  - Layouts <br />
      `Including layouts that wrapping children components`
  - material <br />
      `Simple material design`
  - Todo <br />
      `Shows managind redux and mobx data.`
  - unit-test <br />
      `Includes functions for unit test and react library test.`
  - User <br />
      `Simple user list page.`
## 7. Shopify solve subscription error
  - Problem <br />
    When customer add a subscription on special products which has several variants, the variant's information doesn't reflected on the order.
  - Solution <br />
    The problem was on shopify recharge theme. The products' syncronization was not affected to that products. To solve this problem, I've creat ruleset on recharge app, added products and syncronized. Then new product with the same product title + "auto renew" will be created. I've changed the prepended string to "SUBSCRIPTION". That's all.
## 6. One Net jobs
  - First Job Description <br />
    The jobs displayed on Google search results are referred to as rich snippets. 
  - Challenges
    1) Adjust the job pages to contain rich snippets.
      [ref for concept url](https://developers.google.com/search/docs/data-types/)
    2) Analyzing & Structured Data Makeup 
      [GoogleStructured Data Markup Helper](https://www.google.com/webmasters/markup-helper/)
      
## 5. Full Stack React, Next.JS, Express, MongoDB Social Bookmark Application
  - Project description
    1) google / twitter OAuth
    2) create user account and username when user signs up for the first time
    3) direct user to [projectname].herokuapp.com/@username when they log in
    4) on their page, a very small header with their profile information. username (they cannot edit), and bio (which they can edit), and followers / following
    5) users can view other users profiles if they have the link to other profiles but cannot edit other profiles
    6) users can follow other users
    7) when you click on the "readwithme" link on the header, maybe it can redirect to that page displaying the users
    
  - Live site & projects <br />
    [Live site](https://sayem-nextjs-vercel.vercel.app/login) <br />
    [Node backend](https://github.com/Cardoso-topdev/sayem-node-server) <br />
    [Next.js front-end](https://github.com/Cardoso-topdev/sayem-nextjs-vercel) <br />
    
  - Challenges
    1) CORS error
        - Used cors() middleware on node server.
    2) Deploying MongoDB, Node server, front-end(Nextjs) on cloud server.
        - Deployed mongodb to atlas, node backend on heroku, and nextjs front-end on vercel. <br /> You can check detailed document from these two repos below. <br />
          [node and backend](https://github.com/Cardoso-topdev/sayem-node-server) <br />
          [front-end](https://github.com/Cardoso-topdev/sayem-nextjs-vercel) <br />
    3) Google OAuth login 
        - Create project on Google Cloud Platform, create Client ID and add domain to origins.
    4) Solving JSON position error.
        - Defined environment variables on Vercel
    5) Make easy to development, test, deployment
        - Used git repository for both of development and deployment.
      - Used environment variables for test.
## 4. Shopify Loyalty Lion SDK API integration
  - Project description <br />
    Integrated customer points/rewards system to shopify store. Added custom rules on Loyality Lion. The rule is adding points when user passed quiz. But it doesn't work properly.
  - Source theme code <br />
    [Shopify theme repository](https://github.com/Cardoso-topdev/advanced-shopify-theme)
    
  - Challenges
    1) Build quiz templates and link with shopify store.
        - Built quiz template by using 'Interact' shopify app. Created quiz result pages on shopify store and linked the result to those pages. And to receive the quiz result, append parameters to the url as like as GET method. Also sent quiz passed signal to Klaviyo shopify app to send templated email to customer and analize customer activities.
    2) Send template email to customer and analize customer activities.
        - Built template emails.
        - Made workflow to track customer activity and send template email to customer.  
        - Create segment to analize and report customer activities.
    3) Integrating customer point && rewards system to shopify store.
        - Added activity rules and tiers for giving points and rewards
        - Added custom rules for extra activities such as passing quiz activity.
        - Integrating custom rule SDK APIs to shopify store. For that hosted new node.js server on heroku.
    4) Solve the CORS error when integrating LL custom rule SDK APIs.
        - Prevent browser pref privacy that makes CORS error, hosted new node server on heroku and send data to the node server and resend to LL instead send data to LL directly.
        - Add cors middle ware to node server.
## 3. Click site UI update <br />
  - Project Description <br />
      Frontend Developer w/ some Frontend Design Experience in Figma
  - Result & project  <br />
    Git repository: [one-click-update-ui](https://github.com/Cardoso-topdev/one-click-update-ui) <br />
    [Live Site](https://oscar-update-click.netlify.app/)
    
## 2. One Net Test task. <br />
  - Project Description <br />
    Webflow Animation + JS Test Projects
  - Result & project <br />
    Git repository: [one-net-landing](https://github.com/Cardoso-topdev/one-net-landing) <br />
    [Live Site](https://oscar-one-net-test.netlify.app/)
    
  - Challenges
    1) Implementing animation with third-party library(Wow.js)
    2) Boost animation within circle. Solved this problem with pure css animation.

## 1. Use Chore 
  - Project Description <br />
    I am seeking a react developer to complete my marketing page.<br />Chore is an iOS app, so what I need is to complete the marketing page.  The marketing page must be mobile adative.
  
  - Result & project <br />
    Git repository: [react-chore](https://github.com/Cardoso-topdev/react-chore) <br/>
    [Live Site](https://usechore.netlify.app/)
   
  - Challenges
    1) Build pixel-perfect, mobile-responsive site from Figma. It should works on <addr>iPhone 5 / SE</addr>
      Used bootstrap, media-query, sass
    2) Large-size image load
      Zipped images using online image zip tools
