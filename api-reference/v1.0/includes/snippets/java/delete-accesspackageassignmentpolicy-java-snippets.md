---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0838cf3ca9993fa0a4c5c174fe68ba3389aa1dd3
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211830"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().entitlementManagement().assignmentPolicies("{accessPackageAssignmentPolicyId}")
    .buildRequest()
    .delete();

```