---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f35bc024763d0700c32f87bbcaf7e19647f4c640c6a47d50dd6b728598378cf6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278522"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OAuth2PermissionGrantCollectionPage oauth2PermissionGrants = graphClient.oauth2PermissionGrants()
    .buildRequest()
    .get();

```