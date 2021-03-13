---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ec52b5288291ea748b8cf07aaaf715c6e905f62
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772231"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var taskDefinitions = await graphClient.Print.TaskDefinitions
    .Request()
    .GetAsync();

```