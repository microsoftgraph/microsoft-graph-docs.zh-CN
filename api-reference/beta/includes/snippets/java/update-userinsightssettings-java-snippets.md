---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a476d678fd867243f8910d9c29eb44d74ee6b77c
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210656"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserInsightsSettings userInsightsSettings = new UserInsightsSettings();
userInsightsSettings.isEnabled = false;

graphClient.users("{userId}").settings().itemInsights()
    .buildRequest()
    .patch(userInsightsSettings);

```