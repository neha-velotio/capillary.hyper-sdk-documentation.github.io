# Hydra SDK

Installing the Hydra SDK will provide you with basic analytics functionality with which you can engage your users. With this SDK you can track users in two ways.
1. [Track User Events](README.md#track-user-events) These are the specific traits of a user such as an email, username, mobile, gender and so on. User Attributes helps target users based on these attributes across devices or installs or to personalize the messages.
2. [Track Behavioral Events](track-behavioral-events.md#track-behavioral-events) This will help you record various actions performed by the users. You can track an event using this api with the event name and its characteristics (attributes/properties).

# SDK integration


## Track User Events

The SDK provides four event tracking APIs to log events for reporting User action events. It allows you to identify visitors, track events, dynamically create events and keep an account of the actions performed by the users, along with any properties that describe the action.

1. [Sign In](README.md#sign-in) 
2. [Sign Up](README.md#sign-up) 
3. [User Update](README.md#user-update) 
4. [Sign Out](README.md#sign-out) 

There should be a unique id associated with each user whenever user signs in or signs up in the app. Sdk designates this identifier as cuid, it is strongly recommend providing this identifier as it will allow you to track your users across devices and platforms, improving the quality of your behavioral and demographic data

## Sign In

<details><summary>Android</summary>
<p>

```
fun pushUserSignIn(
        cuid: String,
        firstName: String? = null,
        lastName: String? = null,
        email: String? = null,
        phone: String? = null,
        customData: Map<String, Any>? = null)

```

</p>
</details>

<details><summary>IOS</summary>
<p>
</p>
</details>

## Sign Up

<details><summary>Android</summary>
<p>

```text
fun pushUserSignup(
        cuid: String,
        firstName: String,
        lastName: String,
        email: String,
        phone: String,
        customData: Map<String, Any>?
    )

```
</p>
</details>

<details><summary>IOS</summary>
<p>
</p>
</details>

## User Update

<details><summary>Android</summary>
<p>

```text
 fun pushUserUpdate(
        cuid: String,
        firstName: String? = null,
        lastName: String? = null,
        email: String? = null,
        phone: String? = null,
        customData: Map<String, Any>? = null
    ) 

```

</p>
</details>

<details><summary>IOS</summary>
<p>
</p>
</details>

## Sign Out

<details><summary>Android</summary>
<p>

```text
fun pushUserSignOut(
        cuid: String
    )

```

</p>
</details>


