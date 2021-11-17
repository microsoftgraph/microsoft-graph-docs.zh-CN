---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a838b874d5e7842ccb14a3afaa3f6027575292624b312eafa1dcf3e126d5fbae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215736"
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