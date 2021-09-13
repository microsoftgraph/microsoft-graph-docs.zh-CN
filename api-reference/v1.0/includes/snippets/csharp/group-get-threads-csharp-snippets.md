---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07e72bfa456c2e03c7c46adecb4ac008433c69a83ef98501ab66a2ccd0e802bf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277670"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threads = await graphClient.Groups["{group-id}"].Threads
    .Request()
    .GetAsync();

```