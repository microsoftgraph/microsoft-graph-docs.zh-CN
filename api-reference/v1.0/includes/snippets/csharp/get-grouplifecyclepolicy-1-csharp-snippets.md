---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4ffdf28ea0f836d246f300c0aee99ae7e8e54e10e4352a5280a944cd27b1a44
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333492"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupLifecyclePolicy = await graphClient.GroupLifecyclePolicies["{groupLifecyclePolicy-id}"]
    .Request()
    .GetAsync();

```