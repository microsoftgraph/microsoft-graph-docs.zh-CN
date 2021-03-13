---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 572c7829c8ef591e16b4bb454f1bedda29a4033f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789666"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachments = await graphClient.Users["{user-id}"].Outlook.Tasks["{outlookTask-id}"].Attachments
    .Request()
    .GetAsync();

```