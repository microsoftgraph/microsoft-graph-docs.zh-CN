---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6097d9e8c28fff27485f5fc4e38bb0c58acbca0a9e20f8c1c3e05548c89ca98c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162596"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teachers = await graphClient.Education.Classes["{educationClass-id}"].Teachers
    .Request()
    .GetAsync();

```