---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18f6c036ca93145dfed85a3209642654501271e1
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210346"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryAuditCollectionPage directoryAudits = graphClient.auditLogs().directoryAudits()
    .buildRequest()
    .get();

```