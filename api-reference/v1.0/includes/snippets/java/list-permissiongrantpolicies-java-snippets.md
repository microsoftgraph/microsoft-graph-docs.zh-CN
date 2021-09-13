---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 098b5bfcdc287e576b7b51e30fe7ef628e3fb8f80fae42d82b27c375ea95f248
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409493"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PermissionGrantPolicyCollectionPage permissionGrantPolicies = graphClient.policies().permissionGrantPolicies()
    .buildRequest()
    .get();

```