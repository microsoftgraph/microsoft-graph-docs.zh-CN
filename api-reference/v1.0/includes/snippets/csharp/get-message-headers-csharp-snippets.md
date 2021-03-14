---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40aac464b934061248ac04b522745fc63745a595
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790035"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["{message-id}"]
    .Request()
    .Select("internetMessageHeaders")
    .GetAsync();

```