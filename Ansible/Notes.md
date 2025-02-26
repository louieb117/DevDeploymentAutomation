# Operating Guide


To generate devuser key locally
```
ansible-playbook generate_ssh_key.yaml
```

to run backend server configs
```
ansible-playbook -i inventory/inventory.ini playbooks/site.yaml -u root --ask-pass  
```

to run server configs
```
ansible-playbook -i inventory.ini backend.yaml frontend.yaml
```

to encrypt a string
copy return text
```
❯ ansible-vault encrypt_string --ask-vault-pass 'string to encrypt' --name 'variable'
New Vault password: 
Confirm New Vault password: 
Encryption successful
'variable': !vault |
          $ANSIBLE_VAULT;1.1;AES256
          31326536393163663630373832363438333830373561313133326235353533636630336631316563
          6637633862303066346666353336393965386531663630370a623566353335663735383132373239
          39386536343437636462666463626463333934393366646139383466306335386437353866386434
          3538653935343431390a383038636338373939323136323063376538636530393631646330376461
          37353661313461373934343334626635636665363762316535653036356535316564356233666634
          6161383834336564383065663162383162663431393165616363
```
