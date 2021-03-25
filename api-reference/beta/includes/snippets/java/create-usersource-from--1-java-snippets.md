---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b37642ac53b9d79f8de5471369e6d8d4185148d
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210350"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserSource userSource = new UserSource();
userSource.email = "megan@contoso.com";
userSource.includedSources = EnumSet.of(SourceType.MAILBOX,SourceType.SITE);

graphClient.compliance().ediscovery().cases("4c8f8f70-7785-4bd4-b296-c98376a2c5e1").custodians("2192ca408ea2410eba3bec8ae873be6b").userSources()
    .buildRequest()
    .post(userSource);

```