---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5123354cc245033c9839ee5f33171cfdeda7c55c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "60946253"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedGroupSource unifiedGroupSource = new UnifiedGroupSource();
unifiedGroupSource.additionalDataManager().put("group@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/groups/b96f95c5-b1b3-4142-b039-8ac79e7d2c84"));
unifiedGroupSource.includedSources = EnumSet.of(SourceType.MAILBOX,SourceType.SITE);

graphClient.compliance().ediscovery().cases("15d80234-8320-4f10-96d0-d98d53ffdfc9").custodians("8904528fef4d4578b44f71a80188f400").unifiedGroupSources()
    .buildRequest()
    .post(unifiedGroupSource);

```