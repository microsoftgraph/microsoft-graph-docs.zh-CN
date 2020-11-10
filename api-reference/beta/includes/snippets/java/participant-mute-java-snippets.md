---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd13470ebe3456a64cf51c9b9519fdb609900ec5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968742"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String clientContext = "d45324c1-fcb5-430a-902c-f20af696537c";

graphClient.communications().calls("57dab8b1-894c-409a-b240-bd8beae78896").participants("2765eb15-01f8-47c6-b12b-c32111a4a86f")
    .mute(clientContext)
    .buildRequest()
    .post();

```