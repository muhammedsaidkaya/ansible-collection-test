# Ansible Collection - muhammed.kaya

Documentation for the collection.


# Install 
```
ansible-galaxy collection install git+https://github.com/muhammedsaidkaya/muhammed.kaya.git,master

```

# Example Usage
```
- name: test my new module
  hosts: localhost
  tasks:
    - name: run the new module
      muhammed.kaya.deneme:
        name: 'hello'
        new: true
      register: testout
    - name: dump test output
      debug:
        msg: '{{ testout }}'
```
