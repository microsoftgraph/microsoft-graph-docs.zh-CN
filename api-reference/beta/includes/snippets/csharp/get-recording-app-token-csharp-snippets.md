---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 27ccc4a7b6162f5156c7bd5bbe037aa2fc2eecbf
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665332"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Users["{user-id}"].OnlineMeetings["{onlineMeeting-id}"].Recording
    .Request()
    .GetAsync();

```