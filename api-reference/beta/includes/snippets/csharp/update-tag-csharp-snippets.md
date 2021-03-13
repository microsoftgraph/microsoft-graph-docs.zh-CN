---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5900ca13ce88f8cf9dee6f6ae23ba963182b3666
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776415"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tag = new Microsoft.Graph.Ediscovery.Tag
{
    Description = "This is an updated description."
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Tags["{ediscovery.tag-id}"]
    .Request()
    .UpdateAsync(tag);

```