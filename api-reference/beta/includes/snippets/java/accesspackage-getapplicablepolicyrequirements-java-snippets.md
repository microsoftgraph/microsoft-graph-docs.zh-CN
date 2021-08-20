---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1263833e257c3d488856a7aa0e69af12ae96d5f5
ms.sourcegitcommit: 22bd45d272681658d46a8b99af3c3eabc7b05cb1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2021
ms.locfileid: "58384109"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().entitlementManagement().accessPackages("fb449cf8-3a59-4d86-bdfd-a1b7299681de")
    .getApplicablePolicyRequirements()
    .buildRequest()
    .post();

```