---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0d08cce404fccff5feaaee2563b96ee155d997e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128846"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Remove-MgDirectoryDeletedItem -DirectoryObjectId $directoryObjectId

```