# Spring Cloud Configuration Service :books: #
_Microservice to provide a configuration service._

##Table of Contents##
*******

 1. [Starting](#starting)
 2. [Compile project](#compile-project)
 3. [Pre-requisites](#pre-requisites)
 4. [Building whit](#building-with)
 5. [Installation](#installation)
 6. [Testing](#testing)
 7. [License](#license)
 8. [Authors](#authors)

*******

### Starting ###
Clone project.
`
git clone https://github.com/golivaresh/mc-config-server.git
`

### Compile project :pick: ###

Compile with maven 3.6.1:

```
   1. Access the folder "../mc-config-server/src/java-maven/mc-config-server" from the root folder of the project.
      Execute:
      > mvn clean package
```

### Pre-requisites ###

Things that are needed to install the software.

   * Pending...

### Building with: :hammer_and_pick: ###
(Tools used for construction, example:)

* [Apache Maven 3.6.1](https://maven.apache.org/) - Dependency manager

### Installation :rocket: ###

*For test in eclipse*
    1. Configure the spring.config.location and spring.cloud.bootstrap.location arguments with your personal paths.
    2. Configure the environment variable "ENVIRONMENT" (in this example there are two options: "native" or "dev").
    3. Configure the environment variable "GIT_URL_CONFIGURATION" with the configuration git repository url, example: https://gitlab.com/golivaresh/.
    3. Configure the environment variable "GIT_USERNAME" with the username for authenticate in git repository .
    3. Configure the environment variable "GIT_PASSWORD" with the secret password for authenticate in git repository.
    4. Run the project.
    5. Pending more details...

### Testing :memo: ###

For testing execute:

*is UP?*

```
curl -X GET -d '{}' 'http://localhost:8888/actuator/health'
```

*Get the properties for application*


```
curl -X GET -d '{}' 'http://localhost:8888/client-service/dev'
```


### License :page_facing_up: ###
~~
This project is under license [GNU General Public License](https://www.gnu.org/licenses/gpl-3.0.html).

See the file [LICENSE.md](LICENSE.md) for more details.
~~ 

### Authors :nerd_face: ###

* **Gustavo Olivares Hernández** - *Initial work* - [golivaresh](https://github.com/golivaresh)
