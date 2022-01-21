---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5ecc357efc6a09ee524722c1b44b91f3baa19f0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133921"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgDomainServiceConfigurationRecord -DomainId $domainId

```