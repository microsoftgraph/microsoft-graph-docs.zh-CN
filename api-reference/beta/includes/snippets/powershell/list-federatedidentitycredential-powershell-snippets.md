---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f33fae22cfd1bc374ccdafc81e989b6cbe5c019
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62103889"
---
```powershell

Import-Module Microsoft.Graph.Applications

Get-MgApplicationFederatedIdentityCredential -ApplicationId $applicationId

```