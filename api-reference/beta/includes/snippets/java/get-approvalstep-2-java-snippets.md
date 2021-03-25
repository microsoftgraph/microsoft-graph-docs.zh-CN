---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 659cdea555c54ad5aadf2071915ee46e12e20014
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208659"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ApprovalStep approvalStep = graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentApprovals("abd306ef-f7b2-4a10-9fd1-493454322489").steps("d4fa4045-4716-436d-aec5-57b0a713f095")
    .buildRequest()
    .get();

```