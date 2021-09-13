---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd02cf419c6c0dd10575fd2766f8d577544723698b8b49dd4e291e9ad30c4b84
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106719"
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