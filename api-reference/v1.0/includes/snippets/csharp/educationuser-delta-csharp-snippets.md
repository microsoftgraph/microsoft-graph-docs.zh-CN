---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ab476ff601a7a9749068ac1a0c4c80a9eee0f4eb3a673b9d65155f406e67648
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104980"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Education.Users
    .Delta()
    .Request()
    .GetAsync();

```