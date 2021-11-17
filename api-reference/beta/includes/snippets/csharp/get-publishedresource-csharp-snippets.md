---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 652a050553907170c3eba394ce99ca45bd441a8500e64c8584d0a856234eb37d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218457"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var publishedResource = await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].PublishedResources["{publishedResource-id}"]
    .Request()
    .Expand("agentGroups")
    .GetAsync();

```