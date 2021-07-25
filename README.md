# docker-react1

# Create react app 
npx create-react-app <app-name>
cd <app-name>
npm start
  
# When you’re ready to deploy to production, running npm run build will create an optimized build of your app in the build folder
  
RUN dev env
  docker build -t raje2012/web -f Dockerfile.dev .
  # you can remove volumes if needed
  docker run  -p 3000:3000 -v ${PWD}:/app raje2012/web

  
Run dev
  docker-composer up
  
prod 
  docker run  -p 3000:80 -v ${PWD}:/app raje2012/web
