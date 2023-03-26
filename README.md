<a name="readme-top"></a>

<div align="center">

  <img src="http://cdn.vladimir-portfolio.com/shared/images/Favicon_2.png" alt="logo" width="220" height="auto" />
  <a href="https://cdn.vladimir-portfolio.com"><h1>cdn.vladimir-portfolio.com</h1></a>

  <p>
    My cdn made with :heart:
  </p>

<!-- <a href="https://alxishenry.github.io/docs"><strong>Documentation »</strong></a> -->

<h4>
    <a href="https://vladimir-portfolio.com">Go to the site</a>
  <span> · </span>
    <a href="https://github.com/Vladimir9595/CDN/issues">Report a bug</a>
  <span> · </span>
    <a href="https://github.com/Vladimir9595/CDN/issues">I have an idea</a>
  </h4>
</div>

<br />

# :notebook_with_decorative_cover: Summary

-   [:notebook_with_decorative_cover: About the project](#star2-about-the-project)
    -   [:space_invader: Techs](#space_invader-techs)
-   [:toolbox: Getting Started](#toolbox-getting-started)
    -   [:gear: Setup](#gear-setup)
    -   [:gear: Configuration](#gear-config)
    -   [:test_tube: Tests](#test_tube-tests)
    -   [:gear: Crontab](#gear-crontab)
-   [:wave: Contributors](#wave-contributors)

## :star2: About the project

This project is built with PHP. It's a simple cdn to store my images and files.

### :space_invader: Techs

[![Php](https://img.shields.io/badge/php%20-%23323330.svg?&style=for-the-badge&logo=php&logoColor=8b9ed6&color=gray)]()
[![Shell](https://img.shields.io/badge/bash%20-hotpink.svg?&style=for-the-badge&logo=gnu-bash&logoColor=4EAA25&color=gray)]()

## :toolbox: Getting Started

### :gear: Setup

**Clone the repository**

```
git clone https://github.com/Vladimir9595/CDN.git
```

**Launch the setup script, it will do most of the work for you.**

```
bash setup.sh
```

### :gear: Configuration

The first step is to configure dashboard settings. You can do it by editing the `settings.yml` file situated in the root of the project.

```yml
dashboard:
    title: "CDN - IT'S ME"
    subtitle: "COOL CDN FOR COOL PEOPLE"
    description: "A simple cdn to store my images and files"
```

The second step is to configure the `config.php` file. You can do it by editing the `config.php` file situated in the root of the project.

**In this file you can configure some settings like the environment, the maximum file size, etc...**

```php
return [
	/**
	 * Environment settings
	 */
	'APP_ENV' => 'development',

	/**
	 * Files settings
	 */
	'MAX_FILE_SIZE' => "50000000", // value in bytes (default: 50MB)
];
```

### :test_tube: Tests

**Run linters**

```
make lint
```

**Run the tests using the following command**

```
make tests || npm run tests
```

### :gear: Crontab

**To setup a CRON to save your shared files, run the command below:**

```bash
sudo bash utils/cron.sh || make cron
```

## :wave: Contributors

-   **Vladimir Sacchetto** _alias_ [@Vladimir](https://github.com/Vladimir9595)

<!-- ## :page_with_curl: Liens utiles -->

<p align="right">(<a href="#readme-top">back to top</a>)</p>
