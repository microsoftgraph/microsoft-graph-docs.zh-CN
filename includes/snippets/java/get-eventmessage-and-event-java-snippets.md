---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 573615474f59d67ec0be11281a488949988e4cf2
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774632"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = graphClient.me().messages("AAMkADADVj3fyAABZ5hYdAAA=")
    .buildRequest()
    .expand("eventMessage/event")
    .get();

```