---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc89e8ce32478714d53d02368f83d7450eb4dc7c
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439827"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackage accessPackage = new AccessPackage();
accessPackage.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/c0a74b4d-2694-4d5d-a964-1bee4ff0aaf2"));

graphClient.identityGovernance().entitlementManagement().accessPackages("{id}").incompatibleAccessPackages().references()
    .buildRequest()
    .post(accessPackage);

```