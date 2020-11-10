---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7331cac816e38f1128e43489c10a38b5ae2db7c4
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962309"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Alert> valueList = new LinkedList<Alert>();
Alert value = new Alert();
value.assignedTo = "String";
value.closedDateTime = CalendarSerializer.deserialize("String (timestamp)");
LinkedList<String> commentsList = new LinkedList<String>();
commentsList.add("String");
value.comments = commentsList;
AlertFeedback feedback = new AlertFeedback();
value.feedback = feedback;
value.id = "String (identifier)";
AlertStatus status = new AlertStatus();
value.status = status;
LinkedList<String> tagsList = new LinkedList<String>();
tagsList.add("String");
value.tags = tagsList;
SecurityVendorInformation vendorInformation = new SecurityVendorInformation();
vendorInformation.provider = "String";
vendorInformation.vendor = "String";
value.vendorInformation = vendorInformation;

valueList.add(value);
AlertCollectionResponse alertCollectionResponse = new AlertCollectionResponse();
alertCollectionResponse.value = valueList;
AlertCollectionPage alertCollectionPage = new AlertCollectionPage(alertCollectionResponse, null);

graphClient.security().alerts()
    .updateAlerts(valueList)
    .buildRequest()
    .post();

```