---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab9bb523ad38592002a35d17cf973039fc08e0147f55a5ebb9875bd732e1e727
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902923"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ApprovalStep approvalStep = graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentApprovals("abd306ef-f7b2-4a10-9fd1-493454322489").steps("d4fa4045-4716-436d-aec5-57b0a713f095")
    .buildRequest()
    .get();

```