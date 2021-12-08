---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a66cbfc7a9b8146d37c02fd1e17706d77b58e4cf
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61339516"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InsightsSettings insightsSettings = new InsightsSettings();
insightsSettings.isEnabledInOrganization = true;
insightsSettings.disabledForGroup = "edbfe4fb-ec70-4300-928f-dbb2ae86c981";

graphClient.organization("{organizationId}").settings().peopleInsights()
    .buildRequest()
    .patch(insightsSettings);

```