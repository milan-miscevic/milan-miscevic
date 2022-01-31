### Hi there 👋

<!--
**milan-miscevic/milan-miscevic** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

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

```php
$bih = new Country('Bosnia and Herzegovina')
$bihac = new City('Bihać', $bih);

$milan = new Person(
    firstName: 'Milan',
    lastName: 'Miščević',
    birthDate: new DateTimeImmutable('1985-10-11 23:00:00'),
    birthLocation: $bihac,
);

$banjaluka = new City('Banja Luka', $bih);
$milan->moveTo($banjaluka); // 1992

$turboPascal = new ProgrammingLanguage('Turbo Pascal');
$php = new ProgrammingLanguage('PHP');

$milan->learn($turboPascal); // 2001, the first programming language
$milan->learn($php); // 2003, the first web development steps

$etf = new Faculty('Faculty of Electrical Engineering', $banjaluka);
$etf->enroll($milan); // 2004
$etf->graduate($milan); // 2010, engineer's degree
$etf->graduate($milan); // 2020, master's degree

$inRecursion = new Agency('inRecursion', $banjaluka);
$milan->start($inRecursion); // 2015
$milan->close($inRecursion); // 2021

$germany = new Country('Germany');
$berlin = new City('Berlin', $germany);
$milan->moveTo($berlin); // 2021
```