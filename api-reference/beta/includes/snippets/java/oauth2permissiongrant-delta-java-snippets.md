---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e1f0c3886e3200f152a94ca7ba4366aaa98d6d0fa3383024f26e0b33008372b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278937"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OAuth2PermissionGrantDeltaCollectionPage delta = graphClient.oauth2PermissionGrants()
    .delta()
    .buildRequest()
    .get();

```