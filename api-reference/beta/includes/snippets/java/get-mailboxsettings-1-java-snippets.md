---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49beaa4210ca73d13a31eddb8959edd3889e7be5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978438"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailboxSettings mailboxSettings = graphClient.customRequest("/me/mailboxSettings", MailboxSettings.class)
    .buildRequest()
    .get();

```