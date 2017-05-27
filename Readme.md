## ErpNext Setup (refrence https://github.com/frappe/bench)

```
apt-get install python-minimal
wget https://raw.githubusercontent.com/frappe/bench/master/playbooks/install.py
sudo python install.py --develop
```
### If everything goes well without error, frappe should be installed now.
#### change current directory to frappe
```
cd frappe
```
#### Make a new bench of name *site1.local*. For further info on bench check bench commands on github
```
bench new-site site1.local
```
#### install ERPNext
```
bench get-app erpnext https://github.com/frappe/erpnext
bench --site site1.local install-app erpnext
bench start
```
### Open port on locahost in browser as port mention on the terminal.

## Double check the checkboxes. Don’t create any sample data or don’t check any unused or not required feild.
