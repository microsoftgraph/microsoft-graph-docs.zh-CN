---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a85508f05966e735e14f986b481cc8c33fac37b0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134650"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Remove-MgOauth2PermissionGrant -OAuth2PermissionGrantId $oAuth2PermissionGrantId

```