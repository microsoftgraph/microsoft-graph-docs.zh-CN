---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24a33f365cd1578fe0ba6810cbc62efdb034cdf2b7e1e5f6c6b9652893b27b5c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903402"
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