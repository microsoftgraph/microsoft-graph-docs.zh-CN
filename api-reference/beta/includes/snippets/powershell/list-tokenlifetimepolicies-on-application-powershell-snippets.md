---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01330db91b96146fb52ee7bb43e3aa9cd5c6d028
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62121371"
---
```powershell

Import-Module Microsoft.Graph.Applications

Get-MgApplicationTokenLifetimePolicy -ApplicationId $applicationId

```