---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3d7d8398b650c0fa2f378b92b3b9d9347a383be
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981718"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemInsightsSettings itemInsightsSettings = new ItemInsightsSettings();
itemInsightsSettings.disabledForGroup = "edbfe4fb-ec70-4300-928f-dbb2ae86c981";

graphClient.organization("{organizationId}").settings().itemInsights()
    .buildRequest()
    .patch(itemInsightsSettings);

```