---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e01e8db084fafbecc04e18a4b34a1da5f9b1529
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113559"
---
```powershell

Import-Module Microsoft.Graph.Applications

Get-MgApplicationFederatedIdentityCredential -ApplicationId $applicationId -FederatedIdentityCredentialId $federatedIdentityCredentialId

```