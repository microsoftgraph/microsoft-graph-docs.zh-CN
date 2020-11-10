---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9df9a485e9e1d720c10a1666e8cd081be9e7998a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968286"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String destinationPrinterId = "9a3b3956-ce5b-4d06-a605-5b0bd3e9ddea";

graphClient.print().printers("d5ef6ec4-07ca-4212-baf9-d45be126bfbb").jobs("44353")
    .redirect(destinationPrinterId)
    .buildRequest()
    .post();

```