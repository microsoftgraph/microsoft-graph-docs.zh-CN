---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 468c6af37a92ecfb3f148d92d177fa04f09e8f9b5d060fc7d59f34ae767f2828
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105805"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].ConnectorGroups["{connectorGroup-id}"]
    .Request()
    .DeleteAsync();

```