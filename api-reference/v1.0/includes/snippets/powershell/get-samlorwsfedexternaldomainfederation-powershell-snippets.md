---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f5a643a8ca22584854e00dd690d3b81dd051fb0
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315376"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgDirectoryFederationConfiguration -IdentityProviderBaseId $identityProviderBaseId -Filter "domains/any(x: x/id eq 'contoso.com')" 

```