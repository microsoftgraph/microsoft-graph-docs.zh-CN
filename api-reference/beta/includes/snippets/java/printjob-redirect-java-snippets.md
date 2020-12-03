---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d1c63589703a62ffb61de65122931c517ad4778
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49530668"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String destinationPrinterId = "9a3b3956-ce5b-4d06-a605-5b0bd3e9ddea";

graphClient.print().printers("d5ef6ec4-07ca-4212-baf9-d45be126bfbb").jobs("44353")
    .redirect(destinationPrinterId,null)
    .buildRequest()
    .post();

```