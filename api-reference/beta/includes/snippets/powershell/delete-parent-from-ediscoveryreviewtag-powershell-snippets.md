---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54cd2268877bb048f3ff6ad1bcb5027a1482b85b
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446918"
---
```powershell

Import-Module Microsoft.Graph.Security

Remove-MgSecurityCaseEdiscoveryCaseTag -EdiscoveryCaseId $ediscoveryCaseId -EdiscoveryReviewTagId $ediscoveryReviewTagId

```