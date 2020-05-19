---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 399a6dd3b0cccfd43cff0d9e04ca5c425fa0d586
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402249"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = await graphClient.Teams["303d2c1c-f1c5-40ce-b68e-544343d7f42b"].Channels["19:fec4b0f2825d4c8c82abc09027a64184@thread.skype"].Messages["1555375673184"]
    .Request()
    .GetAsync();

```