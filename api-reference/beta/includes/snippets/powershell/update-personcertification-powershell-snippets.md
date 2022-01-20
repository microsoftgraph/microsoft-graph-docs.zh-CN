---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 894ef9959820637dc4484b7fc7bc89ac16f0297d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62093962"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    IssuingAuthority = "International Academy of Marketing Excellence"
    IssuingCompany = "International Academy of Marketing Excellence"
}

Update-MgUserProfileCertification -UserId $userId -PersonCertificationId $personCertificationId -BodyParameter $params

```