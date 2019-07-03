---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bb91a59a9e03b78194022d291c5d2fdea542bcb3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467745"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drive = await graphClient.Drives["{drive-id}"]
    .Request()
    .GetAsync();

```