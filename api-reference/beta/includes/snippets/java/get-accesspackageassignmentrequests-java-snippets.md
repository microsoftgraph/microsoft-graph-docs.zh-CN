---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d24faea6ba552382f10ddc6286f73eb8ac9aa00e11a647534b52f1fc1e79857
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104183"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentRequestCollectionPage accessPackageAssignmentRequests = graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentRequests()
    .buildRequest()
    .filter("(requestState eq 'PendingApproval')")
    .expand("requestor($expand=connectedOrganization)")
    .get();

```