---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2bc1f24d91c5bc6af05548f80cdc24926423b63ab8b7548fe978db7d507eb48f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278018"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var publishedResources = await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].PublishedResources
    .Request()
    .Expand("agentGroups")
    .GetAsync();

```