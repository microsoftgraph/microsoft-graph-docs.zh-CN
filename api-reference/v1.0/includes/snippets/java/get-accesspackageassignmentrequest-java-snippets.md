---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3191e464d91ae968a3ad9e2ab639096f21762a5b
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61340097"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentRequest accessPackageAssignmentRequest = graphClient.identityGovernance().entitlementManagement().assignmentRequests("{accessPackageAssignmentRequestId}")
    .buildRequest()
    .get();

```