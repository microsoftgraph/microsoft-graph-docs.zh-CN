---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 221de9bcd56a0b677e5ab5da46ede05a24dc9a1f
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439325"
---
```powershell

Import-Module Microsoft.Graph.Search

$params = @{
    DisplayName = "Contoso Marketing"
    Description = "The product marketing team"
}

Update-MgExternalConnectionGroup -ExternalConnectionId $externalConnectionId -ExternalGroupId $externalGroupId -BodyParameter $params

```