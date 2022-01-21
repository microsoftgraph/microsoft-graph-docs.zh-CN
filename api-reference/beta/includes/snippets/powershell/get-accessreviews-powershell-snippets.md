---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2069db6c4a6591ffedc356757849e625f483a9f9
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62095130"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

Get-MgAccessReview -Filter "businessFlowTemplateId eq '6e4f3d20-c5c3-407f-9695-8460952bcc68'" -Top 100 -Skip 0 

```