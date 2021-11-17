---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e69eab5ec20b74cf4088abf07a7bb112d97cf5b913ea8a5bcd357cea32b8ba30
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279087"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.SynchronizationProfiles["{educationSynchronizationProfile-id}"]
    .Resume()
    .Request()
    .PostAsync();

```