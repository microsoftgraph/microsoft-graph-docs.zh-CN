---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6fac9e65d3861d094bcaeb8d462727f858c120f3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954353"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> groupIdsList = new LinkedList<String>();
groupIdsList.add("groupIds-value");

graphClient.groups("{id}")
    .checkMemberGroups(groupIdsList)
    .buildRequest()
    .post();

```