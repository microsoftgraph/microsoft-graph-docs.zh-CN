---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b7955e8f2d5839904a5d4b9f8a7829769b9c0c2b
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933836"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onlineMeeting = await graphClient.App.OnlineMeetings["{id}"]
    .Request()
    .GetAsync();

```