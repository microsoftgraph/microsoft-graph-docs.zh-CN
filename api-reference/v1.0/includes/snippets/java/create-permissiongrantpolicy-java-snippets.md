---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 582d2b4ffda10b6c5dfd872d43ab133e500c2c8bc22d5a3198209818f9dd71d9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279729"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PermissionGrantPolicy permissionGrantPolicy = new PermissionGrantPolicy();
permissionGrantPolicy.id = "my-custom-consent-policy";
permissionGrantPolicy.displayName = "Custom application consent policy";
permissionGrantPolicy.description = "A custom permission grant policy to customize conditions for granting consent.";

graphClient.policies().permissionGrantPolicies()
    .buildRequest()
    .post(permissionGrantPolicy);

```