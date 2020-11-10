---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63dc4f21a0926e3f049e5789026109d802b38a45
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970090"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailboxSettings mailboxSettings = graphClient.customRequest("/me/mailboxSettings", MailboxSettings.class)
    .buildRequest()
    .get();

```