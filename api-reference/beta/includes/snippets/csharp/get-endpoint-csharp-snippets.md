---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: edd62e11a9bc70834f9d37c7a987506f50dcfc6cbdfdf2e70ca270cbeee5ba13
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903690"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var endpoint = await graphClient.Groups["{group-id}"].Endpoints["{endpoint-id}"]
    .Request()
    .GetAsync();

```