---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e83e8fc0cc39f73eb09043cc00aefa71cf79eacd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947173"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connector = await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].Connectors["{connector-id}"]
    .Request()
    .GetAsync();

```