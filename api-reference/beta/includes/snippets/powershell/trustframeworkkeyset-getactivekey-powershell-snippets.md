---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 416ddc74f1b6c7af12ced3a6f5658f335ba35e08
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346038"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgTrustFrameworkKeySetActiveKey -TrustFrameworkKeySetId $trustFrameworkKeySetId

```