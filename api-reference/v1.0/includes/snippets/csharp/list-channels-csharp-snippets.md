---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f23b55e6dc51bc1030cac9c547f3cc7d151dc566
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373610"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channels = await graphClient.Teams["{id}"].Channels
    .Request()
    .GetAsync();

```