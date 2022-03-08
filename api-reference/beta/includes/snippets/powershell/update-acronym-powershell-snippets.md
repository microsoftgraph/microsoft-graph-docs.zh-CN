---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e7a07f79a90a837510726d28ed46489210a899ca
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338329"
---
```powershell

Import-Module Microsoft.Graph.Search

$params = @{
    Description = "A deep neural network is a neural network with a certain level of complexity, a neural network with more than two layers."
}

Update-MgSearchAcronym -AcronymId $acronymId -BodyParameter $params

```