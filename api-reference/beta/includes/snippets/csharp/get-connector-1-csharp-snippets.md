---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa7e8250e3de1c6a57ff66b575511026444efc3d657896e595e6f2e2204a5cad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105647"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connector = await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].Connectors["{connector-id}"]
    .Request()
    .GetAsync();

```