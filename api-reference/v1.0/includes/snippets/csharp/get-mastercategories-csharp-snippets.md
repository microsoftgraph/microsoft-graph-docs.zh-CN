---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8b4d4c20cedb526e24a1f0b05d722c8b8d1f7050
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509795"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var masterCategories = await graphClient.Me.Outlook.MasterCategories
    .Request()
    .GetAsync();

```