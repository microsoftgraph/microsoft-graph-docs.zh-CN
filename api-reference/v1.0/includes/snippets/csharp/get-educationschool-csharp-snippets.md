---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a8dcd3fb8743bcfd49cb73f4bb381c518f189d7
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2021
ms.locfileid: "52474883"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSchool = await graphClient.Education.Schools["{educationSchool-id}"]
    .Request()
    .GetAsync();

```