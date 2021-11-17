---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 933e1dc595fad938e864c9f4667a7b2d742508125195f14eed3796150c3df921
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104796"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.SynchronizationProfiles["{educationSynchronizationProfile-id}"]
    .Reset()
    .Request()
    .PostAsync();

```