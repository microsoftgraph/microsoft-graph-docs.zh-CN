---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 937b99b52606b86cb63ad27542b1245a24d947c5
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757772"
---
```powershell

Import-Module Microsoft.Graph.Reports

Get-MgAuditLogSignIn -Filter "(signInEventTypes/any(t: t ne 'interactiveUser'))" -Sort "createdDateTime DESC" -Top 10 

```