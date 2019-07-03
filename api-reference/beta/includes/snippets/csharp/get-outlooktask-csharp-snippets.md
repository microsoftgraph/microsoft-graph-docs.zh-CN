---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 29a15f7f46b4db83d558a34abe8a09f7b5e18edb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479555"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTask = await graphClient.Me.Outlook.Tasks["AAMkADA1MHgwAAA="]
    .Request()
    .Header("Prefer","outlook.timezone=\"Pacific Standard Time\"")
    .GetAsync();

```