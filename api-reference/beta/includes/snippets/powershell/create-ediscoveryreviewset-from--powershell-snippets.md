---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc5026accdcd82179203b2d33284e01626f019b4
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437926"
---
```powershell

Import-Module Microsoft.Graph.Security

$params = @{
    DisplayName = "My review set 2"
}

New-MgSecurityCaseEdiscoveryCaseReviewSet -EdiscoveryCaseId $ediscoveryCaseId -BodyParameter $params

```