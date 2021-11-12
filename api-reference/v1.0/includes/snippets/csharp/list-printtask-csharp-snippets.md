---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f3f112cff3ca628d04e52d7bf9b91fd25fbca69620bdfbc9a9369dacd87b396
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220972"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Print.TaskDefinitions["{printTaskDefinition-id}"].Tasks
    .Request()
    .GetAsync();

```