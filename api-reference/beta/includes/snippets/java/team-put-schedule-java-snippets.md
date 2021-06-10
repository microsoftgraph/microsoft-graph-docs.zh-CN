---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49b2eb051fbba8fdb112ce8b5d6abed4b3b35c50
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870603"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

byte[] schedule = Base64.getDecoder().decode("{   "enabled":true,   "timeZone":"America/Chicago",   "provisionStatus":"Completed",   "provisionStatusCode":null,   "openShiftsEnabled":true,   "swapShiftsRequestsEnabled":true,   "offerShiftRequestsEnabled":true,   "timeOffRequestsEnabled":true,   "timeClockEnabled":true,   "timeClockSettings":{      "approvedLocation":{         "altitude":1024.13,         "latitude":26.13246,         "longitude":24.34616      }   }} ");
    graphClient.teams("871dbd5c-3a6a-4392-bfe1-042452793a50").schedule()
    .buildRequest()
    .put(schedule);

```