---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20dc0a04f218f5426381508761e10ea8d9acd63ca31d94fc97f5738bc8cd756c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104211"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackage accessPackage = new AccessPackage();
accessPackage.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/c0a74b4d-2694-4d5d-a964-1bee4ff0aaf2"));

graphClient.identityGovernance().entitlementManagement().accessPackages("{id}").incompatibleAccessPackages().references()
    .buildRequest()
    .post(accessPackage);

```