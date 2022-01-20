---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5af786b70a43e3751b5a9e5d5ebc0df9ef59f0a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62107823"
---
```powershell

Import-Module Microsoft.Graph.WindowsUpdates

Get-MgWindowsUpdatesUpdatableAsset -Filter "isof('microsoft.graph.windowsUpdates.azureADDevice')" 

```