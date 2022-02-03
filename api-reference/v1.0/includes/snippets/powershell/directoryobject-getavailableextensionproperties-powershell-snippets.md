---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bdaad35094f982859025d10eda7a944ed603f000
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346723"
---
```powershell

Import-Module Microsoft.Graph.DirectoryObjects

$params = @{
    IsSyncedFromOnPremises = "Boolean"
}

Get-MgDirectoryObjectAvailableExtensionProperty -BodyParameter $params

```