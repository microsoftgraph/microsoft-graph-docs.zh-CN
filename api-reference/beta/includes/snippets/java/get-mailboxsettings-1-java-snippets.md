---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 63dc4f21a0926e3f049e5789026109d802b38a45
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867686"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailboxSettings mailboxSettings = graphClient.customRequest("/me/mailboxSettings", MailboxSettings.class)
    .buildRequest()
    .get();

```