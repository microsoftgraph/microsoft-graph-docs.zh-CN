---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4baa1972b72a3aa566cd4dc6420646068ccd6d2b
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446932"
---
```powershell

Import-Module Microsoft.Graph.Applications

Remove-MgOnPremisePublishingProfilePublishedResourceAgentGroupByRef -OnPremisesPublishingProfileId $onPremisesPublishingProfileId -PublishedResourceId $publishedResourceId -OnPremisesAgentGroupId $onPremisesAgentGroupId

```