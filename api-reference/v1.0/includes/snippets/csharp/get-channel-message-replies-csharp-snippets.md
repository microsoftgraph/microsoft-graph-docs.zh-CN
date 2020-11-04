---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e97f93f7f584033cc90415034a3b94f4e75b8f20
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905312"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var replies = await graphClient.Teams["303d2c1c-f1c5-40ce-b68e-544343d7f42b"].Channels["19:fec4b0f2825d4c8c82abc09027a64184@thread.skype"].Messages["1555375673184"].Replies
    .Request()
    .GetAsync();

```