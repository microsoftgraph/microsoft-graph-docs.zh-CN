---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3517bfa0b646c32c1bf8d7bbf8b3af3a83bbc5f8
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446679"
---
```powershell

Import-Module Microsoft.Graph.Security

Get-MgSecurityCaseEdiscoveryCaseReviewSetQuery -EdiscoveryCaseId $ediscoveryCaseId -EdiscoveryReviewSetId $ediscoveryReviewSetId -EdiscoveryReviewSetQueryId $ediscoveryReviewSetQueryId

```