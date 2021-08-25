---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bdce52173d738b2c18ac31c2c246648711312dd4
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58516055"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleEligibilityScheduleInstance unifiedRoleEligibilityScheduleInstance = graphClient.roleManagement().directory().roleEligibilityScheduleInstances("UafX_Qu2SkSYTAJlL-j6HCssmvzcHW1IohFf6Mp3-h9xbmLcN0jrQL5KvCnYihF4-2-e")
    .buildRequest()
    .get();

```