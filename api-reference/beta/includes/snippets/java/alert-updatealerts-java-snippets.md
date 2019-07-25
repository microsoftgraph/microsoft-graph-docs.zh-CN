---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dc40bad1d84acd0f2da1f03abd4425e06f707a21
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855351"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Alert> valueList = new LinkedList<Alert>();
Alert value = new Alert();
value.assignedTo = "String";
value.closedDateTime = "String (timestamp)";
LinkedList<String> commentsList = new LinkedList<String>();
commentsList.add("String");
value.comments = commentsList;
AlertFeedback feedback = new AlertFeedback();
feedback.additionalDataManager().put("@odata.type", new JsonPrimitive("microsoft.graph.alertFeedback"));
value.feedback = feedback;
value.id = "String (identifier)";
AlertStatus status = new AlertStatus();
status.additionalDataManager().put("@odata.type", new JsonPrimitive("microsoft.graph.alertStatus"));
value.status = status;
LinkedList<String> tagsList = new LinkedList<String>();
tagsList.add("String");
value.tags = tagsList;
SecurityVendorInformation vendorInformation = new SecurityVendorInformation();
vendorInformation.provider = "String";
vendorInformation.vendor = "String";
value.vendorInformation = vendorInformation;

valueList.add(value);

graphClient.security().alerts()
    .updateAlerts(valueList)
    .buildRequest()
    .post();

```