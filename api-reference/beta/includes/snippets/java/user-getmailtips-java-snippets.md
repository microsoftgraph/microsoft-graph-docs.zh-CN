---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5edbc3ced7f06ecb0cd173dc90ab606fd84a8ea5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969638"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> emailAddressesList = new LinkedList<String>();
emailAddressesList.add("danas@contoso.onmicrosoft.com");
emailAddressesList.add("fannyd@contoso.onmicrosoft.com");

EnumSet<MailTipsType> mailTipsOptions = EnumSet.of(MailTipsType.AUTOMATIC_REPLIES,MailTipsType.MAILBOX_FULL_STATUS);

graphClient.me()
    .getMailTips(UserGetMailTipsParameterSet
        .newBuilder()
        .withEmailAddresses(emailAddressesList)
        .withMailTipsOptions(mailTipsOptions)
        .build())
    .buildRequest()
    .post();

```