---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0db4b58bcf0727c396f6457be04a8ebefa6f29e3
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58516040"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleEligibilityScheduleRequest unifiedRoleEligibilityScheduleRequest = graphClient.roleManagement().directory().roleEligibilityScheduleRequests("26bc6813-5457-4302-a482-afafd4e2962a")
    .buildRequest()
    .get();

```