---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 271ece1ba8163bf2e6ac590920ac6cb044e4d13d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968523"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PermissionGrantPolicy permissionGrantPolicy = new PermissionGrantPolicy();
permissionGrantPolicy.displayName = "Custom permission grant policy";

graphClient.policies().permissionGrantPolicies("my-custom-consent-policy")
    .buildRequest()
    .patch(permissionGrantPolicy);

```