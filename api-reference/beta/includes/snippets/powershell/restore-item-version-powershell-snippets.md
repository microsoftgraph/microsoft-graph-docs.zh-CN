---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3624dffb8a3133fe3cfa2b419595a8351123b556
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447043"
---
```powershell

Import-Module Microsoft.Graph.Files

Restore-MgDriveItemVersion -DriveId $driveId -DriveItemId $driveItemId -DriveItemVersionId $driveItemVersionId

```