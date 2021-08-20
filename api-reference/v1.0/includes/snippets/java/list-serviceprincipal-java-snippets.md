---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 431e2ec443c287ee8d37fa3ac2e81e260a19b647fa2ba8caadcb5ca35d052d0f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903230"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServicePrincipalCollectionPage servicePrincipals = graphClient.servicePrincipals()
    .buildRequest()
    .get();

```