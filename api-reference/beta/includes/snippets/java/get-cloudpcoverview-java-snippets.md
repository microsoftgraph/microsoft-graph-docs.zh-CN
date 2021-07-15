---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9989a4de2e77309daa917469c9f238cdb2ba4739
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440088"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcOverview cloudPcOverview = graphClient.tenantRelationships().managedTenants().cloudPcsOverview("{cloudPcOverviewId}")
    .buildRequest()
    .get();

```