---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d74ad8513642fd1f6d6d89b0dc430efcf416291138b5e9a8bfe3af2d7328e91
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215796"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PermissionGrantConditionSet permissionGrantConditionSet = new PermissionGrantConditionSet();
permissionGrantConditionSet.permissionType = PermissionType.DELEGATED;
permissionGrantConditionSet.resourceApplication = "00000003-0000-0000-c000-000000000000";

graphClient.policies().permissionGrantPolicies("my-custom-consent-policy").excludes()
    .buildRequest()
    .post(permissionGrantConditionSet);

```