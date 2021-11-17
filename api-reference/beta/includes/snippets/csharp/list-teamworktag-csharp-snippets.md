---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33897f85d6ee90f46f3ce962fd4a9b7421fa107d65377aca65e0fdfee7a0b807
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163605"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tags = await graphClient.Teams["{team-id}"].Tags
    .Request()
    .GetAsync();

```