---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d3be73057f9cb484e1b41654b29e221ef1fed81
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210567"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Alert alert = new Alert();
alert.assignedTo = "String";
alert.closedDateTime = OffsetDateTimeSerializer.deserialize("String (timestamp)");
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