---
copyright: 'Copyright IBM Corp. 2017'
link: 'message'
is: 'published'
---
# Message

A message is an entry in a conversation.

A person can create a message to place into a conversation via an app such as IBM Workspace. An app too can place a message into a conversation acting under its own identity. And of course other people and apps, who are participating in the conversation can see these messages.

Watson Work Services represents a Message with this object.

| property      | type          | description  |
| ------------- |:------------- |:-----|
| id          | ID      | The ID of the message. The ID scalar type represents a unique identifier, often used to refetch an object or as key for a cache. The ID type appears in a JSON response as a String; however, it is not intended to be human-readable. When expected as an input type, any string (such as "4") or integer (such as 4) input value will be accepted as an ID.|
| created     | Date        | Date this message  was created |
| createdBy   | Person    | Person who created this message |
| updated     | Date    | Date this message  was updated |
| updatedBy   | Person | Person who updated this message  |
| content   | String | The body of the message |
| contentType | String | Mime type of the message content  |
| annotations | [String] | A set of optional objects/attachments that are added to a message, called annotations. Each annotation represents meta data that are related to the message. An annotation is represented by a structured format, which can be viewed as a template. There are different annotation types, some are used to store results of cognitive analysys to a message for example. An annotation can be added at message create time or later, as an update.  Apps are currently limited to create only one type of annotation called `generic` |
