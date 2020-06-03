---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 745a169f23a56664bacbb767bfd48b00d12aaec3
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44216002"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{teamId}").schedule().schedulingGroups("{schedulingGroupId}")
    .buildRequest()
    .delete();

```