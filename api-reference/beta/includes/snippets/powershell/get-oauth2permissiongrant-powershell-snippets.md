---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33c440f5e4f7ddc465ccfdabd85eae76e04de969
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62099302"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgOauth2PermissionGrant -OAuth2PermissionGrantId $oAuth2PermissionGrantId

```