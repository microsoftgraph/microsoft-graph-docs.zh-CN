---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 907e9f05fab847d339781db8822ef3cffe3967dc549dbf9c08fc3c386000c857
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105644"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applications = await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].ConnectorGroups["{connectorGroup-id}"].Applications
    .Request()
    .GetAsync();

```