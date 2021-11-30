<!-- markdownlint-disable MD041 -->

```go
// GET https://graph.microsoft.com/v1.0/me/mailfolders/inbox/messages/{message-id}?$expand=attachments

import (
    events "github.com/microsoftgraph/msgraph-sdk-go/me/mailfolders/item/messages/item"
)

mailFolderId := "inbox"
messageId := "AQMkAGUy..."

expand := item.MessageRequestBuilderGetQueryParameters{
    Expand: []string{"attachments"},
}

options := item.MessageRequestBuilderGetOptions{
    Q: &expand,
}

result, err := client
    .Me()
    .MailFoldersById(mailFolderId)
    .MessagesById(messageId)
    .Get(&options)
```
