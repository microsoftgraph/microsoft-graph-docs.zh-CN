---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a845bf2801927fa439721eaa3e14cdb3d9215ba
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976603"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> groupIdsList = new LinkedList<String>();
groupIdsList.add("groupIds-value");

graphClient.me()
    .checkMemberGroups(groupIdsList)
    .buildRequest()
    .post();

```