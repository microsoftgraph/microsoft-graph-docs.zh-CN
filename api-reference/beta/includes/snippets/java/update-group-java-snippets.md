---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b02226da869280f3069f847788c4c39211f0a87
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953744"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
LinkedList<AssignedLabel> assignedLabelsList = new LinkedList<AssignedLabel>();
AssignedLabel assignedLabels = new AssignedLabel();
assignedLabels.labelId = "45cd0c48-c540-4358-ad79-a3658cdc5b88";
assignedLabelsList.add(assignedLabels);
group.assignedLabels = assignedLabelsList;

graphClient.groups("{id}")
    .buildRequest()
    .patch(group);

```