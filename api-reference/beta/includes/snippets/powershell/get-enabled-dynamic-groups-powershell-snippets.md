---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a14ec6f4641a9c12342808f12dc7b2c0f9e6a051
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113462"
---
```powershell

Import-Module Microsoft.Graph.Groups

Get-MgGroup -Filter "mailEnabled eq false and securityEnabled eq true and NOT(groupTypes/any(s:s eq 'Unified')) and membershipRuleProcessingState eq 'On'" -CountVariable CountVar -Property "id,membershipRule,membershipRuleProcessingState" 

```