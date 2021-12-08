---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e41cfe5321a45d20edfe7c88e4e632503b8bbaa6
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61339521"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var insightsSettings = new InsightsSettings
{
    IsEnabledInOrganization = true,
    DisabledForGroup = "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
};

await graphClient.Organization["{organization-id}"].Settings.PeopleInsights
    .Request()
    .UpdateAsync(insightsSettings);

```