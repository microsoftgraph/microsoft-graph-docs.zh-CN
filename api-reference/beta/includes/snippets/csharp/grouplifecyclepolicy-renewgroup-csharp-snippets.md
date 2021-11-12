---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc4a02f13b3391445b40f3b2cb8919ab18ae4758e76c6b7f6b78b939550dab16
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220674"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupId = "ffffffff-ffff-ffff-ffff-ffffffffffff";

await graphClient.GroupLifecyclePolicies
    .RenewGroup(groupId)
    .Request()
    .PostAsync();

```