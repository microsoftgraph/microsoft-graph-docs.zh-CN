---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b4a8a82b276eeb5c4ce955c8e50614035b4bc12
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "60946249"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedGroupSource unifiedGroupSource = new UnifiedGroupSource();
Group group = new Group();
group.mail = "SecretGroup@contoso.com";
unifiedGroupSource.group = group;
unifiedGroupSource.includedSources = EnumSet.of(SourceType.MAILBOX,SourceType.SITE);

graphClient.compliance().ediscovery().cases("15d80234-8320-4f10-96d0-d98d53ffdfc9").custodians("8904528fef4d4578b44f71a80188f400").unifiedGroupSources()
    .buildRequest()
    .post(unifiedGroupSource);

```