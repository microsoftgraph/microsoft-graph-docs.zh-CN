---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0f798167ad4678871b4a2a54f7931d661e9b4e6
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210665"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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