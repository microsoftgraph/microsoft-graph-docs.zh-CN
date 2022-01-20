---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4112702b33541a9bfacbafe2cb6c6832c2db4de9
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088549"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgContactTransitiveMemberOf -OrgContactId $orgContactId

```