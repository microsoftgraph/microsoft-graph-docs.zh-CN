---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0fed65963e6a7919dfb149c2318fb42cc62673c0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48984204"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOnlineMeetingCollectionPage onlineMeetings = graphClient.communications().onlineMeetings()
    .buildRequest()
    .filter("VideoTeleconferenceId eq '123456789'")
    .get();

```