---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f905738e5f9494e305607fba6e290f4b6a20cde4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981149"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AssignmentOrder newAssignmentOrder = new AssignmentOrder();
LinkedList<String> orderList = new LinkedList<String>();
orderList.add("City");
orderList.add("extension_GUID_ShoeSize");
newAssignmentOrder.order = orderList;

graphClient.identity().b2cUserFlows("{id}").userAttributeAssignments()
    .setOrder(IdentityUserFlowAttributeAssignmentSetOrderParameterSet
        .newBuilder()
        .withNewAssignmentOrder(newAssignmentOrder)
        .build())
    .buildRequest()
    .post();

```