---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90a594c7d2d98873df6158bef2b26dcd2377a56eb4778b88279ce49aa2f1df1c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163237"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSchool = await graphClient.Education.Schools["{educationSchool-id}"]
    .Request()
    .GetAsync();

```