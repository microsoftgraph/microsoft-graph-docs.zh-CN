---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be5b0d4473449c49c96b2fb76c6516ffe3ba119c26761ca1ed37aa333774b511
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274145"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tasks = await graphClient.Me.Planner.Tasks
    .Request()
    .GetAsync();

```