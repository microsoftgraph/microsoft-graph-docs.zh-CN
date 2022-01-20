---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c69f0cc5855054edf80549736a7170d90436103
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126130"
---
```powershell

Import-Module Microsoft.Graph.Notes

Get-MgUserOnenoteOperation -UserId $userId -OnenoteOperationId $onenoteOperationId

```