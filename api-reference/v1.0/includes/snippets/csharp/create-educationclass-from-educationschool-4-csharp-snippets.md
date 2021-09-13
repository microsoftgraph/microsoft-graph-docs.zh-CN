---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef852ea3762b4568a5446a69c0a62c5d6766a738e9d13f2fd8d9a9c3ec968ed1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902283"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Schools["{educationSchool-id}"].Users["{educationUser-id}"]
    .Request()
    .DeleteAsync();

```