---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be4af4897cf87f925881998984d55217863946ea
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095163"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserSource userSource = new UserSource();
userSource.email = "admin@M365x809305.onmicrosoft.com";
userSource.includedSources = EnumSet.of(SourceType.MAILBOX,SourceType.SITE);

graphClient.security().cases().ediscoveryCases("b0073e4e-4184-41c6-9eb7-8c8cc3e2288b").custodians("0053a61a3b6c42738f7606791716a22a").userSources()
    .buildRequest()
    .post(userSource);

```