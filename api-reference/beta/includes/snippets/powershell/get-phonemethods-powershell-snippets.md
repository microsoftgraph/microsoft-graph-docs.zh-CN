---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7060a9ce1d5c1fffbfb9a4a79244746415e8353
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62124268"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgUserAuthenticationPhoneMethod -UserId $userId

```