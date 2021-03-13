---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be086da1a9aee17a556ed24d3bbebb27b0b7936c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783073"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var publishedResources = await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].PublishedResources
    .Request()
    .Expand("agentGroups")
    .GetAsync();

```