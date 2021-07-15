---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1d5623220d78dd51aa729417d5850d48f127518
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440198"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcConnection cloudPcConnection = graphClient.tenantRelationships().managedTenants().cloudPcConnections("86789ee0-e31d-4bee-98e6-6f310bd327bb")
    .buildRequest()
    .get();

```