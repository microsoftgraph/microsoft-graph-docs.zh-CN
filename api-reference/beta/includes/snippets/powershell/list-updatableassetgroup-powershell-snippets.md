---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a9e7f9e0a23ab9a50eedde90ccf9b14fae4a534
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62122463"
---
```powershell

Import-Module Microsoft.Graph.WindowsUpdates

Get-MgWindowsUpdatesUpdatableAsset -Filter "isof('microsoft.graph.windowsUpdates.updatableAssetGroup')" 

```