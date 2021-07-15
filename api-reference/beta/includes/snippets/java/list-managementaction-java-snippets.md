---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c29cd5a59434551c98e02e1f3d006f45da426eb3
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442459"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ManagementActionCollectionPage managementActions = graphClient.tenantRelationships().managedTenants().managementActions()
    .buildRequest()
    .get();

```