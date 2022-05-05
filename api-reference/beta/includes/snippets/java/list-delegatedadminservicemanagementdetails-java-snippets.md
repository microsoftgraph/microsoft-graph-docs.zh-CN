---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c4b9754b8171a7deb6c95dacb211cebdaf4ad94
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202380"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DelegatedAdminServiceManagementDetailCollectionPage serviceManagementDetails = graphClient.tenantRelationships().delegatedAdminCustomers("4fdbff88-9d6b-42e0-9713-45c922ba8001").serviceManagementDetails()
    .buildRequest()
    .get();

```