<!-- ### Hi there 👋 -->

<!--
**OxSama/OxSama** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
<!-- <div align="center" >
  <img src="https://media.giphy.com/media/M9gbBd9nbDrOTu1Mqx/giphy.gif" width="100" />
</div> -->



```php
<?php

namespace OxSama;

class About extends Me implements \JsonSerializable
{
    private const GITHUB_URL = 'https://github.com/OxSama';
    private const LINKEDIN_URL = 'https://www.linkedin.com/in/oxsama/';

    public function whoami(): array
    {
        return [
            'name' => 'Mohammed Tag Eldin Ali',
            'title' => 'Senior Software Engineer',
            'location' => 'UAE',
        ];
    }

    public function getCurrentWorkplace(): array
    {
        return [
            'company' => 'Polaris Technology LLC',
            'position' => 'Senior Software Engineer',
            'duration' => $this->calculateDuration('2024-07'),
            'responsibilities' => [
                'Developing enterprise applications',
                'Code review',
                'Implementing secure development practices',
            ]
        ];
    }

    public function getPreviousWorkplaces(): array
    {
        return [
            [
                'company' => 'Maxnet Digital Services',
                'position' => 'Software Engineer',
                'duration' => '2022-2023',
                'highlights' => [
                    'Developed and maintained multiple web applications',
                    'Implemented automated testing practices',
                    'Collaborated with the Sudanese banks on payment and digital transformation solutions',
                ]
            ],
            [
                'company' => 'Nile University',
                'position' => 'Teaching Assistant',
                'duration' => '2022-2023',
                'highlights' => ['Taught programming fundamentals and provided mentorship to students']
            ],
            [
                'company' => 'Sudan University For Science & Technology',
                'position' => 'Teaching Assistant',
                'duration' => '2022-2023',
                'highlights' => ['Assisted in teaching computer science courses and labs']
            ]
        ];
    }

    public function getTechnicalSkills(): array
    {
        return [
            'languages' => [
                'PHP' => ['Laravel'],
                'JavaScript' => ['React', 'Vue.js', 'Node.js'],
                'Java' => ['Spring Boot'],
                'Dart' => ['Flutter'],
                'Python' => ['Django']
            ],
            'databases' => [
                'MySQL',
                'PostgreSQL',
                'MongoDB',
                'Redis'
            ],
            'devops' => [
                'Docker',
                'GitHub Actions'
            ],
            'tools' => [
                'Git',
                'Linux',
                'Apache'
            ]
        ];
    }

    public function getExpertise(): array
    {
        return [
            'Backend Development' => [
                'RESTful APIs',
                'Microservices',
                'Database Design',
                'Performance Optimization',
                'Secure Development Practices',
            ],
            'Frontend Development' => [
                'SPA Architecture',
                'State Management',
                'UI/UX Implementation'
            ],
            'DevOps' => [
                'CI/CD Pipeline Setup',
                'Server Configuration',
                'Monitoring & Logging'
            ]
        ];
    }

    public function getEducation(): array
    {
        return [
            [
                'degree' => 'Bachelor of Science in Computer Science',
                'university' => 'Sudan University For Science & Technology',
                'year' => '2022',
                'achievements' => [
                    'First Class Honours'
                ]
            ]
        ];
    }

    public function getContactInfo(): array
    {
        return [
            'email' => 'mohamed@oxsama.com',
            'linkedin' => self::LINKEDIN_URL,
            'github' => self::GITHUB_URL
        ];
    }

    private function calculateDuration(string $startDate): string
    {
        $start = new \DateTime($startDate);
        $now = new \DateTime();
        $interval = $start->diff($now);

        $years = $interval->y;
        $months = $interval->m;

        if ($years > 0) {
            return sprintf('%d year%s %d month%s',
                $years,
                $years > 1 ? 's' : '',
                $months,
                $months > 1 ? 's' : ''
            );
        }

        return sprintf('%d month%s', $months, $months > 1 ? 's' : '');
    }

    public function jsonSerialize(): array
    {
        return [
            'about' => $this->whoami(),
            'current_workplace' => $this->getCurrentWorkplace(),
            'previous_workplaces' => $this->getPreviousWorkplaces(),
            'technical_skills' => $this->getTechnicalSkills(),
            'expertise' => $this->getExpertise(),
            'education' => $this->getEducation(),
            'contact' => $this->getContactInfo()
        ];
    }
}
```


<hr>


<div id="badges" align="center">
  <a href="https://www.linkedin.com/in/mohamed-taj-eldin-b510791bb/">
    <img src="https://img.shields.io/badge/LinkedIn-blue?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn Badge"/>
  </a>
<!--   <a href="your-youtube-URL">
    <img src="https://img.shields.io/badge/YouTube-red?style=for-the-badge&logo=youtube&logoColor=white" alt="Youtube Badge"/>
  </a> -->
  <a href="https://twitter.com/OX_SAMA">
    <img src="https://img.shields.io/badge/Twitter-blue?style=for-the-badge&logo=twitter&logoColor=white" alt="Twitter Badge"/>
  </a>
</div>

<div align="center">
  <img src="https://komarev.com/ghpvc/?username=OxSama&style=flat-square&color=red" alt=""/>
</div>

<hr>

<div align="center">
  <img src="https://github.com/devicons/devicon/blob/master/icons/java/java-original-wordmark.svg" title="Java" alt="Java" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/react/react-original-wordmark.svg" title="React" alt="React" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/bootstrap/bootstrap-original-wordmark.svg" title="Bootstrap" alt="Bootstrap" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/composer/composer-line-wordmark.svg" title="Composer" alt="Composer" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/flutter/flutter-original.svg" title="Flutter" alt="Flutter" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/debian/debian-original-wordmark.svg" title="Debian" alt="Debian " width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/css3/css3-plain-wordmark.svg"  title="CSS3" alt="CSS" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/html5/html5-original.svg" title="HTML5" alt="HTML" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/javascript/javascript-original.svg" title="JavaScript" alt="JavaScript" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/express/express-original-wordmark.svg" title="JavaScript" alt="JavaScript" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/bulma/bulma-plain.svg" title="Bulma" alt="Bulma" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/mysql/mysql-original-wordmark.svg" title="MySQL"  alt="MySQL" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/nodejs/nodejs-original-wordmark.svg" title="NodeJS" alt="NodeJS" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/bash/bash-original.svg" title="Bash" alt="Bash" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/git/git-original-wordmark.svg" title="Git" alt="Git" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/docker/docker-original-wordmark.svg" title="Docker" alt="Docker" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/laravel/laravel-plain-wordmark.svg" title="Laravel" alt="Laravel" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/linux/linux-original.svg" title="Linux" alt="Linux" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/php/php-original.svg" title="PHP" alt="PHP" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/ubuntu/ubuntu-plain-wordmark.svg" title="Ubuntu" alt="Ubuntu" width="40" height="40"/>&nbsp;
</div>


<hr>

[![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=OxSama&theme=react)](https://github.com/anuraghazra/github-readme-stats)



<hr>

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=OxSama&layout=compact&theme=react)](https://github.com/anuraghazra/github-readme-stats)

<hr>

#[![GitHub Streak](http://github-readme-streak-stats.herokuapp.com?user=OxSama&theme=react)](https://git.io/streak-stats)

[![GitHub Streak](https://streak-stats.demolab.com/?user=OxSama)](https://git.io/streak-stats)

<hr>

<div align="center">
  <img src="https://media.giphy.com/media/KyIaRm6jYlAGyJ86zH/giphy.gif" width="600" height="300"/>
</div>

