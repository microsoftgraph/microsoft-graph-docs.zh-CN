---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fec86e6290caa246b713b285a555f73c1d834fbf
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882670"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=representation"));

Alert alert = new Alert();
alert.assignedTo = "String";
alert.closedDateTime = "String (timestamp)";
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
    .buildRequest( requestOptions )
    .patch(alert);

```