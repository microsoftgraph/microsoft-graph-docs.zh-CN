---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2bffcb6bb93d1ee631b933bddd367d4d6e68f3e3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956583"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Schools["{educationSchool-id}"].Users["{educationUser-id}"]
    .Request()
    .DeleteAsync();

```