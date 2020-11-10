---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0392b633576572b5a871be89ea889df9d76e4884
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972424"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().printers("{id}")
    .getCapabilities()
    .buildRequest()
    .post();

```