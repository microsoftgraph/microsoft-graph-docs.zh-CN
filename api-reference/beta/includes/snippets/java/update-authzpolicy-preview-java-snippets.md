---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89ef36cb1a125ca02ae870d6b89bf7b80b1f6e3e6ef983f6fa146ca4c039faef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903166"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthorizationPolicy authorizationPolicy = new AuthorizationPolicy();
LinkedList<String> enabledPreviewFeaturesList = new LinkedList<String>();
enabledPreviewFeaturesList.add("assignGroupsToRoles");
authorizationPolicy.enabledPreviewFeatures = enabledPreviewFeaturesList;

graphClient.policies().authorizationPolicy("authorizationPolicy")
    .buildRequest()
    .patch(authorizationPolicy);

```