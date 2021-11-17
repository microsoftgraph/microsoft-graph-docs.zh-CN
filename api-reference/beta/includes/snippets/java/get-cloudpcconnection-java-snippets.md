---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2002f10c12465cec57361f558ee2e8562a8520787b4ad3f8636e6de12915540
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332489"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcConnection cloudPcConnection = graphClient.tenantRelationships().managedTenants().cloudPcConnections("86789ee0-e31d-4bee-98e6-6f310bd327bb")
    .buildRequest()
    .get();

```