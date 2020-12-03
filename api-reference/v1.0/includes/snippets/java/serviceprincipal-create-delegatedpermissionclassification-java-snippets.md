---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be9f71e0052a5e154e6223a2b4989246108201a4
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523091"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DelegatedPermissionClassification delegatedPermissionClassification = new DelegatedPermissionClassification();
delegatedPermissionClassification.permissionId = "e1fe6dd8-ba31-4d61-89e7-88639da4683d";
delegatedPermissionClassification.permissionName = "User.Read";
delegatedPermissionClassification.classification = PermissionClassificationType.LOW;

graphClient.servicePrincipals("{id}").delegatedPermissionClassifications()
    .buildRequest()
    .post(delegatedPermissionClassification);

```