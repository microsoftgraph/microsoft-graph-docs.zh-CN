---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8801c9429481f8bb2fa2bff44ebf035049804302b058760999ab31502b44fe19
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219911"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserInsightsSettings userInsightsSettings = new UserInsightsSettings();
userInsightsSettings.isEnabled = false;

graphClient.users("{userId}").settings().itemInsights()
    .buildRequest()
    .patch(userInsightsSettings);

```