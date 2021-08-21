---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e74b9df243cbe322fad2ad7e68d19320a7ba2f4765403df0683290740941ad97
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219930"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleScheduleInstances = await graphClient.RoleManagement.Directory
    .RoleScheduleInstances("parameterValue","parameterValue","parameterValue","parameterValue")
    .Request()
    .GetAsync();

```