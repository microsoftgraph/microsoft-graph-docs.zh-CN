---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff1521c85f6d40892c3fbe75b3ffbbd17bff8cb8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942823"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Alert alert = new Alert();
alert.assignedTo = "String";
alert.closedDateTime = CalendarSerializer.deserialize("String (timestamp)");
LinkedList<String> commentsList = new LinkedList<String>();
commentsList.add("String");
alert.comments = commentsList;
alert.feedback = AlertFeedback.UNKNOWN;
alert.status = AlertStatus.UNKNOWN;
LinkedList<String> tagsList = new LinkedList<String>();
tagsList.add("String");
alert.tags = tagsList;
SecurityVendorInformation vendorInformation = new SecurityVendorInformation();
vendorInformation.provider = "String";
vendorInformation.vendor = "String";
alert.vendorInformation = vendorInformation;

graphClient.security().alerts("{alert_id}")
    .buildRequest()
    .patch(alert);

```