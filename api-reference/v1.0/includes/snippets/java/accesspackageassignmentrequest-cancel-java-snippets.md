---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43c9fe664748d4b4259c936dfc32a650288385e9
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61337930"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().entitlementManagement().assignmentRequests("{accessPackageAssignmentRequestId}")
    .cancel()
    .buildRequest()
    .post();

```