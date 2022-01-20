---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a863ce10ec8693120813d33b3b50807556f111c7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62091077"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

Remove-MgAccessReviewReviewer -AccessReviewId $accessReviewId -AccessReviewReviewerId $accessReviewReviewerId

```