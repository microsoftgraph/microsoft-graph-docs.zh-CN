---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 664876d435cc96ebab336427cc71089fc54fcd09
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66445069"
---
```powershell

Import-Module Microsoft.Graph.Files

Invoke-MgCheckoutDriveItem -DriveId $driveId -DriveItemId $driveItemId

```