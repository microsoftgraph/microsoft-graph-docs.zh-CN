---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bea76e7194ddb0735c5de2e5ec2f27f982155410
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920639"
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