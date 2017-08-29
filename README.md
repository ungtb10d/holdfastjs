Example usage:

```
import DroneClient from 'drone-js';

// drone server and credentials
const server = "https://drone.company.com";
const token = "...";

// creates the drone client
const client = new DroneClient(server, token);

// fetches the repository list
client.getRepoList().then((repos) => {

});
```

Configure the client from the window:

```
window.DRONE_SERVER = "https://drone.company.com";
window.DRONE_TOKEN = "...";

const client = DroneClient.fromWindow();
```

Configure the client from the environment:

```
process.env.DRONE_SERVER = "https://drone.company.com";
process.env.DRONE_TOKEN = "...";

const client = DroneClient.fromEnviron();
```

Package commands:

```
npm run lint   # lint the codebase
npm run format # format the codebase
```