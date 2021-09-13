---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 59f7343cbaf3c51cd59d0dbadfd1c2d50c5e6f53e66b22c4ed4127e71d766f55
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218409"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryAuditCollectionPage directoryAudits = graphClient.auditLogs().directoryAudits()
    .buildRequest()
    .get();

```