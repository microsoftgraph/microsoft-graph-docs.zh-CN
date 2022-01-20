---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a30c27b473426368a35109b3dd0f1bd4c1b28bef
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133425"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

Get-MgUserOnlineMeetingRegistrationCustomQuestion -UserId $userId -OnlineMeetingId $onlineMeetingId -MeetingRegistrationQuestionId $meetingRegistrationQuestionId

```