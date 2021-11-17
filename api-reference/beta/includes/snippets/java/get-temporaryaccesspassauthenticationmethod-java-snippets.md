---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 127108a09ce5e57f51db16cc2a787a047dbac7307a541bd0fdb861a0753be929
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378594"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TemporaryAccessPassAuthenticationMethod temporaryAccessPassAuthenticationMethod = graphClient.users("kim@contoso.com").authentication().temporaryAccessPassMethods("30fd0dfc-0dfc-30fd-fc0d-fd30fc0dfd30")
    .buildRequest()
    .get();

```