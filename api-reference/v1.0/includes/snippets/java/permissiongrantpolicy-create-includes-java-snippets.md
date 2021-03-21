---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8593729c35f3eb287c355f2b5c17954a95b95c9b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975762"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PermissionGrantConditionSet permissionGrantConditionSet = new PermissionGrantConditionSet();
permissionGrantConditionSet.permissionType = PermissionType.DELEGATED;
permissionGrantConditionSet.clientApplicationsFromVerifiedPublisherOnly = true;

graphClient.policies().permissionGrantPolicies("{id}").includes()
    .buildRequest()
    .post(permissionGrantConditionSet);

```