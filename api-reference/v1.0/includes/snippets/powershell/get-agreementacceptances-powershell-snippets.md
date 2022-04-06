---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4bf5ffd0939923a1749f86816715563eeb5d400b
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63515827"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

# A UPN can also be used as -UserId.
Get-MgUserAgreementAcceptance -UserId $userId

```