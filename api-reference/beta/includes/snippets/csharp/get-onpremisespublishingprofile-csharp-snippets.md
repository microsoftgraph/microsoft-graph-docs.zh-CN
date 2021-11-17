---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36e66ca35d276c56aec7cc985fd8acfd8ac6dfbc0ad8ef0cd1d9c25ce16cede6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219441"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onPremisesPublishingProfile = await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"]
    .Request()
    .Expand("agentGroups")
    .GetAsync();

```