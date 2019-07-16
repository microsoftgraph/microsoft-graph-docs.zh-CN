---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 22e9e161db499230e238f2a8b8bc325922b1e0ab
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736008"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rejectedSenders = await graphClient.Groups["{id}"].RejectedSenders
    .Request()
    .GetAsync();

```