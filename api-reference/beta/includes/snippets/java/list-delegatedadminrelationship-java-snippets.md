---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0417e6d1bc5b0852b18ef508c29532272d55a8d
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210895"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DelegatedAdminRelationshipCollectionPage delegatedAdminRelationships = graphClient.tenantRelationships().delegatedAdminRelationships()
    .buildRequest()
    .get();

```