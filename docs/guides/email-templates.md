# Email Templates <small></small>

> Templates can be used to add custom templates for your emails, or to override the system emails used for things like
> resetting a password or inviting a user.

## 1. Create a template file

Custom email templates are stored in the `templates` folder in your extensions folder. Every template is a
[`liquid`](https://liquidjs.com) file that can render whatever you want!

```
/extensions/templates/<template-name>.liquid
```

To replace a system template with your own, simply name it `password-reset` or `user-invitation` for the password reset
or user invite emails respectively.

::: tip Variables

When overriding the default email templates, make sure to include the <code v-pre>{{ url }}</code> variable somewhere. A
password reset email wouldn't be that useful without the link to go reset your password!

:::
