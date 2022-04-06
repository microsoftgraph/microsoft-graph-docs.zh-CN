---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61010a0b386141c294fe85d250e807e782de0fca
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516060"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ApprovalStage approvalStage = new ApprovalStage();
approvalStage.reviewResult = "Approve";
approvalStage.justification = "OK";

graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentApprovals("abd306ef-f7b2-4a10-9fd1-493454322489").stages("d4fa4045-4716-436d-aec5-57b0a713f095")
    .buildRequest()
    .patch(approvalStage);

```