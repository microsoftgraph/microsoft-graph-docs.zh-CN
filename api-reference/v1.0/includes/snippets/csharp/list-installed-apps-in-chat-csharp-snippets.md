---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4de9a015212b63fbb5a2ffbf7ff680e11cd533e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958494"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Chats["{chat-id}"].InstalledApps
    .Request()
    .GetAsync();

```