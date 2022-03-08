---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3366d70525460d47b86c871556f309c9b4054fee
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338315"
---
```powershell

Import-Module Microsoft.Graph.Search

$params = @{
    DisplayName = "DNN"
    StandsFor = "Deep Neural Network"
    Description = "A deep neural network is a neural network with a certain level of complexity, a neural network with more than two layers."
    WebUrl = "http://microsoft.com/deep-neural-network"
    State = "draft"
}

New-MgSearchAcronym -BodyParameter $params

```