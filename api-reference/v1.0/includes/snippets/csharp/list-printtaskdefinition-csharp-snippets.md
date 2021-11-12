---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec157d6b1a9439f8bdd4014c6ff42f1a98bb34b807e883d0f8625906f11b410d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106030"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var taskDefinitions = await graphClient.Print.TaskDefinitions
    .Request()
    .GetAsync();

```