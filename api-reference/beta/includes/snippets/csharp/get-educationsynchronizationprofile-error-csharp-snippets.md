---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2157da840a810df2474cb5546be64915d6aa6ddd992029b5671f2b076300082c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219764"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var errors = await graphClient.Education.SynchronizationProfiles["{educationSynchronizationProfile-id}"].Errors
    .Request()
    .GetAsync();

```