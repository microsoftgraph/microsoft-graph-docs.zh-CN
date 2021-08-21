---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62c90146ff35a9d208a4188aa16a82c6662883d64d5fff0e09b844e070fcc860
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158446"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.roleManagement().directory().roleAssignmentScheduleRequests("{unifiedRoleAssignmentScheduleRequestsId}")
    .cancel()
    .buildRequest()
    .post();

```