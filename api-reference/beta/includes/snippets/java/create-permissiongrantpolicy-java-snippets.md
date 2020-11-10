---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ddab776ccb2eb8aa5344ad505efa698398fb164d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969445"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PermissionGrantPolicy permissionGrantPolicy = new PermissionGrantPolicy();
permissionGrantPolicy.id = "my-custom-consent-policy";
permissionGrantPolicy.displayName = "Custom application consent policy";
permissionGrantPolicy.description = "A custom permission grant policy to customize conditions for granting consent.";

graphClient.policies().permissionGrantPolicies()
    .buildRequest()
    .post(permissionGrantPolicy);

```