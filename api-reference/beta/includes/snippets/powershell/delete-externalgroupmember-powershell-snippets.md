---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f02a18099c92b9a31cf8a92bdbb66918514be9e
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439641"
---
```powershell

Import-Module Microsoft.Graph.Search

Remove-MgExternalConnectionGroupMember -ExternalConnectionId $externalConnectionId -ExternalGroupId $externalGroupId -IdentityId $identityId

```