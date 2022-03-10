---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d6687a8f290da1c34a73f0cd86b33e448cf97ce
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412129"
---
```powershell

Import-Module Microsoft.Graph.DirectoryObjects

$params = @{
    IsSyncedFromOnPremises = $true
}

Get-MgDirectoryObjectAvailableExtensionProperty -BodyParameter $params

```