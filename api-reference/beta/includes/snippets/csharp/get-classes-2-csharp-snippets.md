---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33a0798c4ec4da0c9b593012b73e1f0a40dedf281b6cb3839c0db4bf8b43a07e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332301"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var classes = await graphClient.Education.Schools["{educationSchool-id}"].Classes
    .Request()
    .GetAsync();

```