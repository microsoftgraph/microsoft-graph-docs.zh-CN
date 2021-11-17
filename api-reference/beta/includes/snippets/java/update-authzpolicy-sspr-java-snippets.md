---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: adef3d1cc13fc5028b05aca7d0d372786cd9e01a6b917198b5b7db4285dcb8ac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903168"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthorizationPolicy authorizationPolicy = new AuthorizationPolicy();
authorizationPolicy.allowedToUseSSPR = true;

graphClient.policies().authorizationPolicy("authorizationPolicy")
    .buildRequest()
    .patch(authorizationPolicy);

```