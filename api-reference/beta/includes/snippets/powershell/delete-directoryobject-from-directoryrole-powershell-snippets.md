---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 824aba3db3bca3edebaf91e15a5f743d567e2233
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437981"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Remove-MgDirectoryRoleMemberByRef -DirectoryRoleId $directoryRoleId -DirectoryObjectId $directoryObjectId

```