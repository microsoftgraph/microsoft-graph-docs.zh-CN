---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 562720d2b52aeb6f1a981d94277c2001d1b04cca
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62125564"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Remove-MgDirectoryFederationConfiguration -IdentityProviderBaseId $identityProviderBaseId

```