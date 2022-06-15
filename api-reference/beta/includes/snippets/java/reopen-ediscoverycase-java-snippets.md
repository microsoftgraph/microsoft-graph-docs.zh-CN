---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e52a94c7a058a88102e6fa7ec7ef286b736c7bc
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092930"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.security().cases().ediscoveryCases("061b9a92-8926-4bd9-b41d-abf35edc7583")
    .reopen()
    .buildRequest()
    .post();

```