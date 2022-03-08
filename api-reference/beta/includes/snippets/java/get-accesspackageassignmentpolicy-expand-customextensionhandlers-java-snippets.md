---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e38665119cbaf063d5d7f4773ab83d0c27f5e0ff
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333048"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentPolicy accessPackageAssignmentPolicy = graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentPolicies("4540a08f-8ab5-43f6-a923-015275799197")
    .buildRequest()
    .expand("customExtensionHandlers($expand=customExtension)")
    .get();

```