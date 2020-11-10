---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7adc016bddb48ad94379163eb90f03d990bbf0f9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961595"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AudioRoutingGroup audioRoutingGroup = graphClient.communications().calls("{id}").audioRoutingGroups("{id}")
    .buildRequest()
    .get();

```