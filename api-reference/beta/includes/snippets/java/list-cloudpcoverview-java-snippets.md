---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 945d30fbf24b652b1f8d3f0c201f5efc1a72495d95918e71b97dca9474756bfb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158526"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcOverviewCollectionPage cloudPcsOverview = graphClient.tenantRelationships().managedTenants().cloudPcsOverview()
    .buildRequest()
    .get();

```