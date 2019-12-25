---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a0d3037d98561d6776af10d5ce7c6d7a1918686
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865835"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RejectReason reason = RejectReason.BUSY;

graphClient.communications().calls("57dab8b1-894c-409a-b240-bd8beae78896")
    .reject(reason,null)
    .buildRequest()
    .post();

```