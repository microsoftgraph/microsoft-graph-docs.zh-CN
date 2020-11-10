---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b480eb984c022fef14f624054ac58ea077e814b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979977"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkPosition workPosition = graphClient.me().profile().positions("{id}")
    .buildRequest()
    .get();

```