---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81aeec114c913f2fb461b7267687410dcfab3a5b
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61334910"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().entitlementManagement().accessPackages("{accessPackageId}")
    .getApplicablePolicyRequirements()
    .buildRequest()
    .post();

```