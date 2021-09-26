---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bfd8bf5455cbebaf2c71556ef47dc386b63be499
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59929130"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ClaimsMappingPolicy claimsMappingPolicy = new ClaimsMappingPolicy();
claimsMappingPolicy.displayName = "UpdateClaimsPolicy";

graphClient.policies().claimsMappingPolicies("{id}")
    .buildRequest()
    .patch(claimsMappingPolicy);

```