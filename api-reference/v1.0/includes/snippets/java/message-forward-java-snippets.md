---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55a3a8b48a80d342ddc8140d7eeb2a147ce3fc92
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980712"
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

graphClient.me().messages("{id}")
    .forward(MessageForwardParameterSet
        .newBuilder()
        .withToRecipients(toRecipientsList)
        .withMessage(null)
        .withComment(comment)
        .build())
    .buildRequest()
    .post();

```