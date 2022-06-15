---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4aea93d78887912fbfc93a3ebfa4e81977282314
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093490"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoveryCustodian ediscoveryCustodian = new EdiscoveryCustodian();
ediscoveryCustodian.email = "AdeleV@contoso.com";

graphClient.security().cases().ediscoveryCases("{ediscoveryCaseId}").custodians()
    .buildRequest()
    .post(ediscoveryCustodian);

```