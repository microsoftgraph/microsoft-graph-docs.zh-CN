---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5290af3415ae2dd133ed1da72aaf0ea84a2fc7f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976155"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedApproval privilegedApproval = new PrivilegedApproval();
privilegedApproval.userId = "userId-value";
privilegedApproval.roleId = "roleId-value";
privilegedApproval.approvalType = "approvalType-value";
privilegedApproval.approvalState = ApprovalState.PENDING;
privilegedApproval.approvalDuration = DatatypeFactory.newInstance().newDuration("datetime-value");

graphClient.privilegedApproval()
    .buildRequest()
    .post(privilegedApproval);

```