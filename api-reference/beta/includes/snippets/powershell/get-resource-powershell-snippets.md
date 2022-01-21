---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6965db0cdfe5003d8fbf0deb072b3d692516d2ae
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129525"
---
```powershell

Import-Module Microsoft.Graph.Notes

Get-MgUserOnenoteResourceContent -UserId $userId -OnenoteResourceId $onenoteResourceId

```