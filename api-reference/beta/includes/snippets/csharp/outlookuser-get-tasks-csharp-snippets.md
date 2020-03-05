---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e151c63db240b9181eeed7f73e56b777310cbf4a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37637528"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Me.Outlook.Tasks
    .Request()
    .GetAsync();

```