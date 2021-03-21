---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b1acc5363a17c97d9cf6323e93bb678810305139
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967496"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Recipient> toRecipientsList = new LinkedList<Recipient>();
Recipient toRecipients = new Recipient();
EmailAddress emailAddress = new EmailAddress();
emailAddress.address = "danas@contoso.onmicrosoft.com";
emailAddress.name = "Dana Swope";
toRecipients.emailAddress = emailAddress;

toRecipientsList.add(toRecipients);

String comment = "Dana, hope you can make this meeting.";

graphClient.me().events("{id}")
    .forward(EventForwardParameterSet
        .newBuilder()
        .withToRecipients(toRecipientsList)
        .withComment(comment)
        .build())
    .buildRequest()
    .post();

```