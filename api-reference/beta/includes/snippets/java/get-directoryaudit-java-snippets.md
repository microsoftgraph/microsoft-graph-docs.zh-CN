---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7c4b3f28be007ef6c5d772fba40ee7017527d08528a4fcb6373b90be18b4a8c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105642"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryAudit directoryAudit = graphClient.auditLogs().directoryAudits("{id}")
    .buildRequest()
    .get();

```