---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 772d01844daa1c84a186b7fbd3104ca3261ddd42
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979737"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrinterShare printerShare = graphClient.print().shares("{id}")
    .buildRequest()
    .get();

```