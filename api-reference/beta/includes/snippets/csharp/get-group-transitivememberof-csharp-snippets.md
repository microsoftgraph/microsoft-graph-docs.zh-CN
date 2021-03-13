---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21f245a1a25cea935b21b5d2cabbf4e6e79c66e8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781147"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transitiveMemberOf = await graphClient.Groups["{group-id}"].TransitiveMemberOf
    .Request()
    .GetAsync();

```