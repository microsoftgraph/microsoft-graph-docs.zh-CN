---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a766aca58507bd78f9dd79a69140ac173e84d29
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475390"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Education.Users
    .Request()
    .GetAsync();

```