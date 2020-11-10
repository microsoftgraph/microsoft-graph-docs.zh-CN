---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2333d5b82aff2ee7032a4400ba43519be95bf219
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959975"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().calendarGroups("{id}")
    .buildRequest()
    .delete();

```