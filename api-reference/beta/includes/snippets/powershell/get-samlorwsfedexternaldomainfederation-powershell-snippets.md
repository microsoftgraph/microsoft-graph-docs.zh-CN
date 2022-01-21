---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f5a643a8ca22584854e00dd690d3b81dd051fb0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62105520"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgDirectoryFederationConfiguration -IdentityProviderBaseId $identityProviderBaseId -Filter "domains/any(x: x/id eq 'contoso.com')" 

```