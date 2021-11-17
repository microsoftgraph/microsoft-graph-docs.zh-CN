---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d58811eb8cb39da49b1ea36b64ddffee72849f9c93ac2b0ab0f982a188a71e9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215731"
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