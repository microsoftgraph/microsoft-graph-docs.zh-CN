---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf90de312aa53d7363bbc3a7d43b237b69642732
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62121209"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgIdentityConditionalAccessPolicy -Filter "displayName eq 'SimplePolicy1' or displayName eq 'SimplePolicy2'" 

```