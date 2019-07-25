---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8f60c6685e77ce133210e16a93c3728f0cc5f8c9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862508"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryAuditCollectionPage directoryAudits = graphClient.auditLogs().directoryAudits()
    .buildRequest()
    .get();

```