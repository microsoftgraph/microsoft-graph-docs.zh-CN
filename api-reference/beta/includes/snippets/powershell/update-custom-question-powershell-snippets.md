---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b6b670e33e1d0ef75bcedbadef75455b3136b06
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62102790"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    AnswerInputType = "radioButton"
    AnswerOptions = @(
        "Software Engineer"
        "Software Development Manager"
        "Product Manager"
        "Data scientist"
        "Other"
    )
}

Update-MgUserOnlineMeetingRegistrationCustomQuestion -UserId $userId -OnlineMeetingId $onlineMeetingId -MeetingRegistrationQuestionId $meetingRegistrationQuestionId -BodyParameter $params

```