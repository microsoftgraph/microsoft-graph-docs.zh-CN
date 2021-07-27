---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c388ec2b3077e115b8dd29184619e6dedb4f4d0
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53581365"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentRequestCollectionPage accessPackageAssignmentRequests = graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentRequests()
    .buildRequest()
    .filter("(requestState eq 'PendingApproval')")
    .expand("requestor($expand=connectedOrganization)")
    .get();

```