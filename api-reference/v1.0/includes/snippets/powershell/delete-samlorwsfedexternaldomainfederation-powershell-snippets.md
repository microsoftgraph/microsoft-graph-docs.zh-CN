---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 562720d2b52aeb6f1a981d94277c2001d1b04cca
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315364"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Remove-MgDirectoryFederationConfiguration -IdentityProviderBaseId $identityProviderBaseId

```