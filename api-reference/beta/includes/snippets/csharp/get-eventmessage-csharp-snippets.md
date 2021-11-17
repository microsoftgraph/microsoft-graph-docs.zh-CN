---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2941218f68268aaf5dd427668f39b7ef837abfddd2a880613bc7adf2811fe600
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277458"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["{message-id}"]
    .Request()
    .GetAsync();

```