---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 41dbc2d23ebfbeb704c8b9db300667985573353e1f1d95ee8c6b6069165c7de9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163338"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.TrustFramework.Policies["{trustFrameworkPolicy-id}"]
    .Request()
    .DeleteAsync();

```