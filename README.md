## giveasone.org

#### High-level requirements
- [x] Domain (giveasone.org through AWS)
- [x] Host (AWS EC2)
- [x] SSL (via let’s encrypt)
- [x] Email notifications (via AWS SES)
- [x] Backend framework (Django)
- [ ] Frontend framework
- [ ] Database engine
- [ ] 3rd party payments (do we still want to use Stripe?)

#### Homepage requirements
- [ ] Navigation (about us, terms of use, privacy policy, account, donate, login)
- [x] Logo
- [ ] High-level description of how giveasone works
- [ ] High-level descriptions of each charity giveasone supports
- [ ] Bar graph (or similar) for showing total donations and matches for all charities

#### Donation page requirements
- [ ] Initial donation field
- [ ] Maximum donation field
- [ ] A list of available charities w/ sliders representing the percentage of donations to each charity. By default, all charities will split the donations evenly (see Humble Bundle)
- [ ] Each charity should have a brief description with a link to a seperate page for that charity (and/or the charity’s home page)
- [ ] A button that opens the 3rd party payment platforms page
- [ ] An e-mail should be sent once the donation has been submitted and confirmed

#### User account page requirements
- [ ] Ability to reset password
- [ ] Ability to ask for refend for any previous donation that has not been matched
- [ ] Log of all previous donations and matches
- [ ] Ability to access receipts for tax purposes?

#### About us page requirements
- [ ] High level description of how giveasone works
- [ ] Detailed description of how giveasone works

#### Data model requirements
##### User
* email
* first, last name

##### transaction
* id
* 3rd party payment reference id
* user
* timestamp
* total_donated

#### giveasone donation algorithm


### To discuss
* Project communication (slack, github, irc, matrix, something else?)
* Non-profit status
* Legal requirements and protections
* CI (coala-bears)
* Coding standards (type hints?)
* Python version 3.7?