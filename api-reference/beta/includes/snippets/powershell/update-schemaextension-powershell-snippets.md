---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ebb5e9e0540ee7965d20446d7aafaf7704726a67
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212071"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
}

Update-MgUser -UserId $userId -BodyParameter $params

```