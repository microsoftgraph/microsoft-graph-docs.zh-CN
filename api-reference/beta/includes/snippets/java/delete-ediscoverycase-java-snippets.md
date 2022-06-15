---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62830373d73f21bd6f158d8578a75fdaae9c2d02
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095981"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.security().cases().ediscoveryCases("22aa2acd-7554-4330-9ba9-ce20014aaae4")
    .buildRequest()
    .delete();

```