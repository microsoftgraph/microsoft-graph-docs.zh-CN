---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d1b5aba1932a75a5ad6c83a5d227af4c803157c
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659036"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedGroupSource unifiedGroupSource = new UnifiedGroupSource();
unifiedGroupSource.additionalDataManager().put("group@odata.bind", new JsonPrimitive("/groups/000044f9-47c8-4a87-bccf-291fbf006a54"));
unifiedGroupSource.includedSources = EnumSet.of(SourceType.MAILBOX,SourceType.SITE);

graphClient.compliance().ediscovery().cases("{ediscoveryCaseId}").custodians("{custodianId}").unifiedGroupSources()
    .buildRequest()
    .post(unifiedGroupSource);

```