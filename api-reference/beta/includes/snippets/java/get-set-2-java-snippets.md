---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c667d834ef719945c36491e646f69342c5e86c68
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580494"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Set set = graphClient.termStore().sets("8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f")
    .buildRequest()
    .get();

```