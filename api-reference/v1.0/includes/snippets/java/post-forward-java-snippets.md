---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eea7e75bd7c5ca716e810df46908d975fff64315
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981021"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "comment-value";

LinkedList<Recipient> toRecipientsList = new LinkedList<Recipient>();
Recipient toRecipients = new Recipient();
EmailAddress emailAddress = new EmailAddress();
emailAddress.name = "name-value";
emailAddress.address = "address-value";
toRecipients.emailAddress = emailAddress;

toRecipientsList.add(toRecipients);

graphClient.groups("{id}").threads("{id}").posts("{id}")
    .forward(PostForwardParameterSet
        .newBuilder()
        .withComment(comment)
        .withToRecipients(toRecipientsList)
        .build())
    .buildRequest()
    .post();

```