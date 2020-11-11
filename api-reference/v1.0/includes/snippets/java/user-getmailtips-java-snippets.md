---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e529af33f792aedf0e56250706227afeb2771c28
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48984117"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> emailAddressesList = new LinkedList<String>();
emailAddressesList.add("danas@contoso.onmicrosoft.com");
emailAddressesList.add("fannyd@contoso.onmicrosoft.com");

EnumSet<MailTipsType> mailTipsOptions = EnumSet.of(MailTipsType.AUTOMATIC_REPLIES,MailTipsType.MAILBOX_FULL_STATUS);

graphClient.me()
    .getMailTips(emailAddressesList,mailTipsOptions)
    .buildRequest()
    .post();

```