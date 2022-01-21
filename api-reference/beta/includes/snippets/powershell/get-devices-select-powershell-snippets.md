---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1094611b6763824754146ec0d312332e143645aa
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133979"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgDevice -Property "id,extensionAttributes" 

```