---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4339e96a683c3b1376fa00c1572c53ce26ffd70
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211351"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DelegatedAdminCustomerCollectionPage delegatedAdminCustomers = graphClient.tenantRelationships().delegatedAdminCustomers()
    .buildRequest()
    .get();

```