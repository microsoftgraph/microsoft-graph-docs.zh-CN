---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8dda7ce15e279c26a567251e453cefd03d37c98316da0395f1977a4561e8d4d6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164271"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcAuditEvent cloudPcAuditEvent = graphClient.deviceManagement().virtualEndpoint().auditEvents("{id}")
    .buildRequest()
    .get();

```