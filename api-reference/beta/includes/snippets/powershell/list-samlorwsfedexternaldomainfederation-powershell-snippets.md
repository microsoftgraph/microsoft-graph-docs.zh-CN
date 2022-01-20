---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82abff65efd2bd166f1474eb08b670818067b94a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132718"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgDirectoryFederationConfiguration -IdentityProviderBaseId $identityProviderBaseId

```