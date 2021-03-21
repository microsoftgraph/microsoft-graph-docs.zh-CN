---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 028b106abfeee1a4780c9ff06f350ad40fa23e36
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981429"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Alert> valueList = new LinkedList<Alert>();
Alert value = new Alert();
value.assignedTo = "String";
value.closedDateTime = OffsetDateTimeSerializer.deserialize("String (timestamp)");
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
    .updateAlerts(AlertUpdateAlertsParameterSet
        .newBuilder()
        .withValue(valueList)
        .build())
    .buildRequest()
    .post();

```