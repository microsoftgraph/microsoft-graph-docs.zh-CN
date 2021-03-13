---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74d28441bc7bd2794b83e4fffc858fb2d45125f8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776660"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var operations = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Operations
    .Request()
    .GetAsync();

```