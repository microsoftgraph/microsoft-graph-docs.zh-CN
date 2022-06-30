---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 59333fe34fd9b10b917526d2915df3ce50458880
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440089"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

Remove-MgEntitlementManagementConnectedOrganizationExternalSponsorByRef -ConnectedOrganizationId $connectedOrganizationId -DirectoryObjectId $directoryObjectId

```