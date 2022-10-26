## CSS modules

- purpose is to give unique className for styling a particular type of component dynamically

### process

- rename CSS file as .module.css
- Instead of conventional css import; import an object name can be anything from that css file
  eg : import styles from ".button.module.css"
- Instead of normal conventional adding classname as className = "button", Now It will added as className = {styles.button}

- It will dynamically gives className to that component as "ComponentName_classname_randomHashCode"

eg : Button_button_xkjsqhd

### Dynamically class adding

- use backtick concept
  className = {`${styles["form-control"]} ${!invalid && styles.invalid}`}
