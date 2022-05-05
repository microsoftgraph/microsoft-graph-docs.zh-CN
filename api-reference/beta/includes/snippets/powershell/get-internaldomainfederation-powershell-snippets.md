---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c14be0ca9d090969ced20041076a8c84cf6a96e5
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212150"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgDomainFederationConfiguration -DomainId $domainId -InternalDomainFederationId $internalDomainFederationId

```