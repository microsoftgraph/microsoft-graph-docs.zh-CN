---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1435cd8e74719fbb13f9a5482df17b77325bd643
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58516037"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.roleManagement().directory().roleAssignmentScheduleRequests("15fec3d4-64b1-4b03-beb7-f1ba6dddf6cc")
    .cancel()
    .buildRequest()
    .post();

```