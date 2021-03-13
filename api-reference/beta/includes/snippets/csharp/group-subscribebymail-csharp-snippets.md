---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53349fd9ddaac5dbc97ca24ed334b7f1bd305bbb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784561"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"]
    .SubscribeByMail()
    .Request()
    .PostAsync();

```