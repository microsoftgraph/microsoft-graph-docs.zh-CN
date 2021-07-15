---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97e13ecc822a7465b96f85c704f9c214d0658a88
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441571"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcConnectionCollectionPage cloudPcConnections = graphClient.tenantRelationships().managedTenants().cloudPcConnections()
    .buildRequest()
    .get();

```