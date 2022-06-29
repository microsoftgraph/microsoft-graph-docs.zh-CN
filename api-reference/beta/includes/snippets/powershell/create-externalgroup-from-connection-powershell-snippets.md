---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76b3197ec8658ec2b584f8bdd4d5f0adf93b9e30
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439718"
---
```powershell

Import-Module Microsoft.Graph.Search

$params = @{
    Id = "31bea3d537902000"
    DisplayName = "Contoso Marketing"
    Description = "The product marketing team"
}

New-MgExternalConnectionGroup -ExternalConnectionId $externalConnectionId -BodyParameter $params

```