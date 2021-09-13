---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 181e4eb3e1838eb0482bbe19e4d9b88a8790757044d77cafcd63ece1e063ac4e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279182"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AssignmentOrder newAssignmentOrder = new AssignmentOrder();
LinkedList<String> orderList = new LinkedList<String>();
orderList.add("City");
orderList.add("extension_GUID_ShoeSize");
newAssignmentOrder.order = orderList;

graphClient.identity().b2xUserFlows("{id}").userAttributeAssignments()
    .setOrder(IdentityUserFlowAttributeAssignmentSetOrderParameterSet
        .newBuilder()
        .withNewAssignmentOrder(newAssignmentOrder)
        .build())
    .buildRequest()
    .post();

```