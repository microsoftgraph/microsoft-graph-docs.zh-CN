---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be759777018e71019e36a12828e23c1e2cb61849
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970463"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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