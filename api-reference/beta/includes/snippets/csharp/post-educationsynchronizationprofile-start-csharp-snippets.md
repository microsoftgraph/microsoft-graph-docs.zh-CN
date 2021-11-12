---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e252a6c5221684e55401934b91c41c0d522c0fe8f4d15520a5eb0718eaa555d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332401"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.SynchronizationProfiles["{educationSynchronizationProfile-id}"]
    .Start()
    .Request()
    .PostAsync();

```