---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0865ef6dba470197abee7d2c8bbdef992460fcde
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774649"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Event event = graphClient.me().calendar().events("AAMkADJXJGu0AABf02qwAAA=")
    .buildRequest()
    .get();

```