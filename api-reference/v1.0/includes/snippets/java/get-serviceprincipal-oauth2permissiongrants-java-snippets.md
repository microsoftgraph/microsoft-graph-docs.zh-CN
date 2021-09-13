---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a55fa84b3e30224a69ad687c65413a3560ce7fa6f988d7d05f3167402ca859d0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333212"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OAuth2PermissionGrantCollectionWithReferencesPage oauth2PermissionGrants = graphClient.servicePrincipals("{id}").oauth2PermissionGrants()
    .buildRequest()
    .get();

```