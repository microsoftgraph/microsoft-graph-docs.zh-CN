---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc7192df0d27b79b05acbd04787fec333feb2ff8
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347843"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    KeyId = "f0b0b335-1d71-4883-8f98-567911bfdca6"
}

Remove-MgApplicationPassword -ApplicationId $applicationId -BodyParameter $params

```