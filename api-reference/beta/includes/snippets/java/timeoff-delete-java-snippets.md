---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8c7443f1c7c6cd08949d80d732619d098de93118
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868075"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{teamId}").schedule().timesOff("{timeOffId}")
    .buildRequest()
    .delete();

```