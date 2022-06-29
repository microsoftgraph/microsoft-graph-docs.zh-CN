---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 222a8e60686a2fdfee11e51bf05b13e54e512a5c
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66445104"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Remove-MgDirectoryAdministrativeUnitMemberByRef -AdministrativeUnitId $administrativeUnitId -DirectoryObjectId $directoryObjectId

```