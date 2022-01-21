---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e078b1eaaa0b84d10242bf22c72948f24d283fd
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089865"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    "@odata.type" = "#microsoft.outlookServices.openTypeExtension"
    ExtensionName = "Com.Contoso.Estimate"
    CompanyName = "Contoso"
    ExpirationDate = "2016-07-30T11:00:00.000Z"
    DealValue = 
    TopPicks = @(
        "Employees only"
        "Add spouse or guest"
        "Add family"
    )
}

Update-MgGroupThreadPostExtension -GroupId $groupId -ConversationThreadId $conversationThreadId -PostId $postId -ExtensionId $extensionId -BodyParameter $params

```