---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b99ecd93c7275a20f962d6cb5393abb0829d74cb64aad790cd2d69bb32a5e097
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57331898"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TenantCustomizedInformationCollectionPage tenantsCustomizedInformation = graphClient.tenantRelationships().managedTenants().tenantsCustomizedInformation()
    .buildRequest()
    .get();

```