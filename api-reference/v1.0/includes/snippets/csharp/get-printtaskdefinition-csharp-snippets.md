---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2fa3c1759447e5d37b88e822660a317c70bc32d1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50768706"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printTaskDefinition = await graphClient.Print.TaskDefinitions["{printTaskDefinition-id}"]
    .Request()
    .GetAsync();

```