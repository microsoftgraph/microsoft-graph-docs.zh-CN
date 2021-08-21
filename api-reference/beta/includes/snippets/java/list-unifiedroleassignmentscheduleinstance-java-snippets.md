---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b27d379c855a4d612b0a2dd1b69ee8f8d8ca91b698926b051df4fb1785db32c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103925"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentScheduleInstanceCollectionPage roleAssignmentScheduleInstances = graphClient.roleManagement().directory().roleAssignmentScheduleInstances()
    .buildRequest()
    .get();

```