---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac68605a7425fb8418af1aa6f47d9d5fbdf129e942d0d15cd38acd2bc62d5dd2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220348"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OAuth2PermissionGrantCollectionWithReferencesPage oauth2PermissionGrants = graphClient.users("7d54cb02-aaa3-4016-9f9c-a4b49422dd9b").oauth2PermissionGrants()
    .buildRequest()
    .get();

```