---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a76ee180cfbe243187b40d8e3ee63528b5867ef
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61348788"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PermissionGrantConditionSet permissionGrantConditionSet = new PermissionGrantConditionSet();
permissionGrantConditionSet.permissionType = PermissionType.DELEGATED;
permissionGrantConditionSet.certifiedClientApplicationsOnly = true;

graphClient.policies().permissionGrantPolicies("{id}").includes()
    .buildRequest()
    .post(permissionGrantConditionSet);

```