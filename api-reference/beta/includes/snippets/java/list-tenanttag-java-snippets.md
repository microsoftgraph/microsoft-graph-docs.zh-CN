---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1596a856870cd3e0025b88304f5f64f436ac27de294ab2065ba0d0e0681693f2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220876"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TenantTagCollectionPage tenantTags = graphClient.tenantRelationships().managedTenants().tenantTags()
    .buildRequest()
    .get();

```