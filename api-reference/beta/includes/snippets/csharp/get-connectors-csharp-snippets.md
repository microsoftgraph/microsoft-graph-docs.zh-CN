---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3323b90a2d37391fa5b2c0bbca3b23f74f483de4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802342"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectors = await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].Connectors
    .Request()
    .GetAsync();

```