---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b447c4470e598e32e809fa3232ce60bc0cf1e80a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972452"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().printers("1a5f91a7-9bd1-4d5f-bb86-f43554cac51c").taskTriggers("25be207e-1154-491f-aa68-a9f7007d4bec")
    .buildRequest()
    .delete();

```