---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 68fd44a6d7e3b42c0f75e22cddcca89478d12b94
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867635"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> emailAddressesList = new LinkedList<String>();
emailAddressesList.add("danas@contoso.onmicrosoft.com");
emailAddressesList.add("fannyd@contoso.onmicrosoft.com");

MailTipsType mailTipsOptions = MailTipsType.AUTOMATIC_REPLIES;

graphClient.me()
    .getMailTips(emailAddressesList,mailTipsOptions)
    .buildRequest()
    .post();

```