# Hive
Coding on Hive

Feching data from Hive

Initial Installation
- Install Python 3
- To check python version (in window cmd) ```python --version```
- Installing Beem Module to Interact with Hive
- - In window cmd ```python -m pip install beem```

Checking the Current RC Balance of a Hive Account (Ref: https://ecency.com/programming/@learncode/part-5-coding-on-hive-with-python-working-with-resource-credits)

```import beem

ACCOUNT_NAME = input('Enter account name: ')

acc = beem.account.Account(ACCOUNT_NAME)
mana = acc.get_rc_manabar()['current_mana']
print('Current mana for @%s is %d RCs' % (ACCOUNT_NAME, mana))
```

My code for checking voting power of an account is as follow

```
import beem

account = beem.account.Account('Your Account Name here')
vp = account.get_voting_power()
print('Current mana for @%s is %.2f RCs' % (account, vp))

```
