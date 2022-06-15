---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 495952810c69f01376240a468ae430c07ead62a4
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095976"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.security().cases().ediscoveryCases("{ediscoveryCaseId}").custodians("{ediscoveryCustodianId}")
    .activate()
    .buildRequest()
    .post();

```