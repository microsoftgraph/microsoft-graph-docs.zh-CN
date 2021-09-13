---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef58fc6bc5327fda629e80b1c4da9b73a171d83202151924023651afea293fce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162997"
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