---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 237eac907a3741ee1ffd50b83987519645e42810
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66443493"
---
```powershell

Import-Module Microsoft.Graph.Files

Get-MgDriveItemChild -DriveId $driveId -DriveItemId $driveItemId

```