---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae6466ae8319558af3d2ff4a093223f38ee28d0f
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53578824"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.applications("{id}")
    .unsetVerifiedPublisher()
    .buildRequest()
    .post();

```