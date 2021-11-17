---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed63355fb6ca679c047a50115625e880ceb113848acbe0c3c04fb16273368426
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163599"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var trustFrameworkKeySet = await graphClient.TrustFramework.KeySets["{trustFrameworkKeySet-id}"]
    .Request()
    .GetAsync();

```