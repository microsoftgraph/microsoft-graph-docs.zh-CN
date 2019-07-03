---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ea6a0dafb64aab774d78c98e4d60e82f3a93894e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467515"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "view";

var scope = "anonymous";

await graphClient.Me.Drive.Items["{item-id}"]
    .CreateLink(type,scope)
    .Request()
    .PostAsync();

```