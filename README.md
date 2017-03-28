1) create new ember addon and define a reducers folder

    ember addon themes

2) add this new addon as a dependency (look in the yelp package.json)

    "themes": "file:../themes"

3) from the addon (if you want to make changes/ etc)

    npm link

4) then from the ember app

    npm link themes

5) now import the reducer from the addon

open the yelp (ember app) reducers/index.js file

    import theme from 'themes/reducers/theme';

6) now boot the ember app (from the yelp directory)

    ember s
