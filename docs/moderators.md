# Moderators

Moderators help manage and verify new map submissions.

## Moderator Goals:

- [x] Verify the automatic validation
- [x] Test each new map to make sure there aren't issues that need to be resolved
- [x] Check for any problematic content or descriptions

### Tips:

- The validation bot will automatically post a comment that contains substantial information.
- The validation bot links to a `map-preview` asset that is automatically uploaded, containing a 2d preview image of the map.

## Moderator Slash Commands:

Moderators can perform the following action commands when operating in a map submission Issue:

### Requesting a re-validation

If something gets stuck, or a user modifies the (optional) Map Description after an earlier validation occurred,
a moderator may request a re-validation by adding a new comment with the contents:

```
/replace validation
```

> Note: There is _no need_ to manually request a validation if someone issues a `/replace map-upload` and uploads a fixed map - a validation pass will automatically be queued.

### Approving a map submission

To approve a map submission, the map must first have passed validation (i.e. the bot should have posted a validation with the **Status: `Pass`**).

In this validation message posted by the bot, you'll see instructions on posting an approval command as a new comment:

```
/approve
```

## (For Admins): Adding moderators:

Moderators are simply GitHub accounts that have been granted `triage` permissions on this repo.
