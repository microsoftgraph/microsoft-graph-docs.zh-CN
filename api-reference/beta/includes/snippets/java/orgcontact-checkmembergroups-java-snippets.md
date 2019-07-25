---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 995a4b1e3d28de884c8b35db0d2eb5615ac8a8e8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878052"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> groupIdsList = new LinkedList<String>();
groupIdsList.add("groupIds-value");

graphClient.contacts("{id}")
    .checkMemberGroups(groupIdsList)
    .buildRequest()
    .post();

```