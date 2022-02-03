---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a1200b2bc7c08a1b1d51dc5eacc05512619096e
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351394"
---
```powershell

Import-Module Microsoft.Graph.PersonalContacts

$params = @{
    ParentFolderId = "AQMkADIxYjJiYgEzLTFmNjYALTRjYTMtODA1NC0wZDkxZGNmOTcxNTQALgAAA8RJzXYaLKZPlmn0ge0edZkBADa3qi2IMXRNg6RwQSHe_F8AAAIBDgAAAA=="
    DisplayName = "Important contacts"
}

# A UPN can also be used as -UserId.
New-MgUserContactFolder -UserId $userId -BodyParameter $params

```