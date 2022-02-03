---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc826906e969518f0a7d732bc11180a7ae607821
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351968"
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

# A UPN can also be used as -UserId.
Update-MgUserOnlineMeetingRegistrationCustomQuestion -UserId $userId -OnlineMeetingId $onlineMeetingId -MeetingRegistrationQuestionId $meetingRegistrationQuestionId -BodyParameter $params

```