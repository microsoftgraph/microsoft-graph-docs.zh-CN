---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 22e9e161db499230e238f2a8b8bc325922b1e0ab
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479155"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rejectedSenders = await graphClient.Groups["{id}"].RejectedSenders
    .Request()
    .GetAsync();

```