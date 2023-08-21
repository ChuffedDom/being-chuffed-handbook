Here, Chuffed will determine the stack of the technology that is default to all builds. 

The vision is to have a quick and effective pipeline of development that serve people before infrastructure. 

What Chuffed seeks to accomplish is:
- A platform agnostic deployment workflow that will require as little code as possible.
- A way of creating MVPs and Prototypes over a period of time and number of people that does not require project management.
- To be deployment first, infrastructure second.

As Chuffed diversifies it's offering for different clients and internal product initiatives, we need to deploy as quick as possible for validation to solutions and providing an offering that is competitive with others. But using a typical stack requires a sizable team, or a large amount of technical knowledge amongst everyone else. Therefore, we are limited by the infrastructure we want to build, and not the result of the output.

## The Default Stack
Chuffed will default to building using:
- **Flutter** for it's cross platform, single code base implementation.
	- **Provider** for state management.
- **Firebase** for it's low cost of entry, speed of access, and global availability.
	- **Hosting** for where web apps live.
	- **Authentication** for all login and sign up tasks.
	- **Firestore** for all database needs.
- **Github** for version control and Actions to deploy to Production and Staging environments.

This stack has proven to be rapid in the process of building MVPs, prototype, and proof of concepts. The ecosystem of third party packages is robust and vetted.
## Architecture
Rather that compartmentalising code by operation, e.g. this file has data storage, that file has components, each file will represent a feature with all of the necessary code within. The structure is as follows.
### Models
Structure data and reformat it for Firebase or other utilisation.
### Logic
The processing of all data and runtime storage, aka state management.
## Render
All Widgets are place here and are called / referenced from main.dart.