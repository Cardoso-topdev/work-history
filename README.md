# My sites <br />
  ## React templates
   - [material-kit](https://material-kit-react-sooty.vercel.app/)   https://material-kit-react-sooty.vercel.app/
   - [fuse theme](https://react-fuse.vercel.app/)   https://react-fuse.vercel.app/
  ## Bootstrap templates
   - [Volt template](https://oscar-volt-bootstrap.netlify.app/)   https://oscar-volt-bootstrap.netlify.app/ <br />
  ## Next.js templates
   - [next.js template1](https://nextjs-template1.vercel.app/)  https://nextjs-template1.vercel.app/ <br />
  
  [typeW](https://typew.com/)     https://typew.com/  <br />
  [gohirenow](https://www.gohirenow.com/)   https://www.gohirenow.com/<br />
  [useChore](https://usechore.netlify.app/)     https://usechore.netlify.app/ <br />
  [workplace landing](https://oscar-workplace-credit.netlify.app/)    https://oscar-workplace-credit.netlify.app/ <br />
  [One net landing](https://oscar-one-net-test.netlify.app/)    https://oscar-one-net-test.netlify.app/ <br />
  [update click](https://oscar-update-click.netlify.app/)     https://oscar-update-click.netlify.app/  <br />
  [next.js sayem](https://sayem-nextjs-vercel.vercel.app/login)   https://sayem-nextjs-vercel.vercel.app/login <br />
  [shopify siete](https://sietefoods.com/)    https://sietefoods.com/ <br />
  
# work-history

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
## 4. Shopify LL SDK API integration
  - Project description <br />
    Integrated customer points/rewards system to shopify store. Added custom rules on LL. The rule is adding points when user passed quiz. But it doesn't work properly.
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
