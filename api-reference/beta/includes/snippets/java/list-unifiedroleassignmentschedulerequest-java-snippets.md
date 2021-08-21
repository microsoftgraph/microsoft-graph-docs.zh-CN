---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b61c5663639edb4360e2859afc29db8e3e8350ae788f7c831ad441ff1a1b2e94
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104473"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentScheduleRequestCollectionPage roleAssignmentScheduleRequests = graphClient.roleManagement().directory().roleAssignmentScheduleRequests()
    .buildRequest()
    .get();

```