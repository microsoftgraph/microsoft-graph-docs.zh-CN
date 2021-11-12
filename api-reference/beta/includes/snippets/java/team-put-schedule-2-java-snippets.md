---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b3aa2bea7f03d29277bd1da55ba4088164e7947d13529af687213f223bd89466
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103932"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

byte[] schedule = Base64.getDecoder().decode("{   "enabled":true,   "timeZone":"America/Chicago",   "provisionStatus":"Completed",   "provisionStatusCode":null,   "openShiftsEnabled":true,   "swapShiftsRequestsEnabled":true,   "offerShiftRequestsEnabled":true,   "timeOffRequestsEnabled":true,   "timeClockEnabled":true,   "timeClockSettings":{      "approvedLocation":{         "altitude":1024.13,         "latitude":26.13246,         "longitude":24.34616      }   }} ");
    graphClient.teams("871dbd5c-3a6a-4392-bfe1-042452793a50").schedule()
    .buildRequest()
    .put(schedule);

```