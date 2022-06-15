---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82ec2543709928d780789462e3284f386260e922
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095583"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.security().cases().ediscoveryCases("b0073e4e-4184-41c6-9eb7-8c8cc3e2288b").custodians("c25c3914f9f743ee9cbaa25377e0cec6")
    .applyHold()
    .buildRequest()
    .post();

```