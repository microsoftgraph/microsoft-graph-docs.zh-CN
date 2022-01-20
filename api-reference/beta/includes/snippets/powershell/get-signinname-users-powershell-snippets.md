---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f4ad2c7abe6ae74c3a04ce29140b30006a82e4c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126645"
---
```powershell

Import-Module Microsoft.Graph.Users

Get-MgUser -Property "displayName,id" -Filter "identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')" 

```