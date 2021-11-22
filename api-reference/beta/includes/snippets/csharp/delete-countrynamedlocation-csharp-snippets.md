---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cdf63b8472eb9565970e09e48b92cc8167a8e2059627266d0a6cb0f48813601
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220322"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.ConditionalAccess.NamedLocations["{namedLocation-id}"]
    .Request()
    .DeleteAsync();

```