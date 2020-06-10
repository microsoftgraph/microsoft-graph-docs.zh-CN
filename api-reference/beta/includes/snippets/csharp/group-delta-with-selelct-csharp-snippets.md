---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c249ce7e8f599a7a2904b36caa14e5b1d0c1000
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684313"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Groups
    .Delta()
    .Request()
    .Select("displayName,description,mailNickname")
    .GetAsync();

```