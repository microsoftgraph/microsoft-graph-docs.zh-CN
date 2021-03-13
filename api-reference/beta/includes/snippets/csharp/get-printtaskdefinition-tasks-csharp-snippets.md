---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c681f96961d5cef18487e946ce86c2336de850c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798214"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Print.TaskDefinitions["{printTaskDefinition-id}"].Tasks
    .Request()
    .GetAsync();

```