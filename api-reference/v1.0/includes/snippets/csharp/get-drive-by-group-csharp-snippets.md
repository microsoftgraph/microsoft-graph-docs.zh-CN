---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6476f7d810f86f3bace7699733665e022ddc493a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805589"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drive = await graphClient.Groups["{group-id}"].Drive
    .Request()
    .GetAsync();

```