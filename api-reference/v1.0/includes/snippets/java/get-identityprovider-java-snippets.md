---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 307fc5b3e4897c3080baeb55ff08892350bd22820cacebd806dceb4a50651e61
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904310"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProvider identityProvider = graphClient.identityProviders("Amazon-OAuth")
    .buildRequest()
    .get();

```