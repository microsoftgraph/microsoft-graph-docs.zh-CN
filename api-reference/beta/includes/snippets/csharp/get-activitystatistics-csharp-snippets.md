---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1334f39accc7938d7851ceef16c83a44988c372368434ba9667caa9deef0e18
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902597"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var activityStatistics = await graphClient.Me.Analytics.ActivityStatistics
    .Request()
    .GetAsync();

```