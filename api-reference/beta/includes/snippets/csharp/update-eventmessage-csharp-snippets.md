---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fcb535e44664ba3fea67ce37dbc20ec012220faa
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2019
ms.locfileid: "36845913"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    IsRead = true
};

await graphClient.Me.Messages["{id}"]
    .Request()
    .UpdateAsync(message);

```