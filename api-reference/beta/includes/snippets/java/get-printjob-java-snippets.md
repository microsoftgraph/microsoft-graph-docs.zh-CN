---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f963456faac9476322ef1ea2f9ec9848b5d3262
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968338"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintJob printJob = graphClient.print().printers("c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb").jobs("5182")
    .buildRequest()
    .get();

```