---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 38229844b8cc0d1e2114456add79d134ff4438f2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101199"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgDirectoryDeletedItem -DirectoryObjectId $directoryObjectId -CountVariable CountVar -Sort "deletedDateTime asc" -Property "id,DisplayName,deletedDateTime" 

```