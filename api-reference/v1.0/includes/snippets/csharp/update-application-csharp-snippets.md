---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1892e4249c36bc9036051aecce0d84020354fad3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798235"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var application = new Application
{
    DisplayName = "New display name"
};

await graphClient.Applications["{application-id}"]
    .Request()
    .UpdateAsync(application);

```