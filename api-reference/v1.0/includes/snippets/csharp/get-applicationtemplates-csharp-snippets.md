---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89fdf13c0347789cdf856eae7228aa2a17c0acfc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775140"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applicationTemplates = await graphClient.ApplicationTemplates
    .Request()
    .GetAsync();

```