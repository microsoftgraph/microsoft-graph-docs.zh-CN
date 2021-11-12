---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd9911badc1b62ad78af780a667e67278455299097583627ff0e34ff7a05b531
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106327"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProvider identityProvider = new IdentityProvider();
identityProvider.clientSecret = "1111111111111";

graphClient.identityProviders("Amazon-OAuth")
    .buildRequest()
    .patch(identityProvider);

```