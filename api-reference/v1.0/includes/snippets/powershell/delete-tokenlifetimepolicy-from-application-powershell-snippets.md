---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a50b1ce8b0e72f29e26796d925755556bb0a58e5
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66445090"
---
```powershell

Import-Module Microsoft.Graph.Applications

Remove-MgApplicationTokenLifetimePolicyByRef -ApplicationId $applicationId -TokenLifetimePolicyId $tokenLifetimePolicyId

```