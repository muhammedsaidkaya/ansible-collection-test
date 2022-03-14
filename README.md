
# Install
```
ansible-galaxy collection install git+https://github.com/muhammedsaidkaya/ansible-collection-test,master

```

# Example Usage
```
- name: test my new module
  hosts: localhost
  tasks:
    - name: run the new module
      kloia.provisioner.deneme:
        name: 'hello'
        new: true
      register: testout
    - name: dump test output
      debug:
        msg: '{{ testout }}'
```