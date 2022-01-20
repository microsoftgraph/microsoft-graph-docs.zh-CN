---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c9c057f36af1ae4a1c74888806d04b48b6637f3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126642"
---
```powershell

Import-Module Microsoft.Graph.Users

Get-MgUser -Property "id,mail,assignedLicenses" -Filter "assignedLicenses/any(u:u/skuId eq cbdc14ab-d96c-4c30-b9f4-6ada7cdc1d46)" 

```