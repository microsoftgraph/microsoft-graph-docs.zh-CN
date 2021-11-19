---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1edf8517e6a7838c079b821edd09b2e2d681d472
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094068"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InsightsSettings insightsSettings = new InsightsSettings();
insightsSettings.disabledForGroup = "edbfe4fb-ec70-4300-928f-dbb2ae86c981";

graphClient.organization("{organizationId}").settings().itemInsights()
    .buildRequest()
    .patch(insightsSettings);

```