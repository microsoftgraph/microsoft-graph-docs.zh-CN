---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9eaf7466bb856940cbbbdb1fb875b5ec093cab29
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49752735"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AssignmentOrder newAssignmentOrder = new AssignmentOrder();
LinkedList<String> orderList = new LinkedList<String>();
orderList.add("City");
orderList.add("extension_GUID_ShoeSize");
newAssignmentOrder.order = orderList;

graphClient.identity().b2cUserFlows("{id}").userAttributeAssignments()
    .setOrder(newAssignmentOrder)
    .buildRequest()
    .post();

```