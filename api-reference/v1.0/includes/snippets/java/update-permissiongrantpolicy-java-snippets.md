---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca47dd951d34837df33038e3d5eb011013029157cc28b1dce9c4d7e6d3338624
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278328"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PermissionGrantPolicy permissionGrantPolicy = new PermissionGrantPolicy();
permissionGrantPolicy.displayName = "Custom permission grant policy";

graphClient.policies().permissionGrantPolicies("my-custom-consent-policy")
    .buildRequest()
    .patch(permissionGrantPolicy);

```