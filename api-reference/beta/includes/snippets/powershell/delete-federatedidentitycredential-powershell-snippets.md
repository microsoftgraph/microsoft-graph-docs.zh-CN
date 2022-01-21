---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78bec3f503e41322323cc04b7deee8b40b0a349b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106136"
---
```powershell

Import-Module Microsoft.Graph.Applications

Remove-MgApplicationFederatedIdentityCredential -ApplicationId $applicationId -FederatedIdentityCredentialId $federatedIdentityCredentialId

```