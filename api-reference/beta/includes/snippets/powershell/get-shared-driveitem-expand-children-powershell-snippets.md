---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69742e3c687ec255fc42f959aaa7024f44de7b38
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62098801"
---
```powershell

Import-Module Microsoft.Graph.Files

Get-MgShareDriveItem -SharedDriveItemId $sharedDriveItemId -ExpandProperty "children" 

```