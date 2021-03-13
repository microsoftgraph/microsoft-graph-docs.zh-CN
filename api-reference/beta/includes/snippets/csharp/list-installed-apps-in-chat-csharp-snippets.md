---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4de9a015212b63fbb5a2ffbf7ff680e11cd533e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770108"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Chats["{chat-id}"].InstalledApps
    .Request()
    .GetAsync();

```