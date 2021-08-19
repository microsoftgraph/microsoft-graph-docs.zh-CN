---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b39c8e055601766a711096e6402effb177278c63f84461c58cc9856d68e2c136
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106370"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chats = await graphClient.Users["{user-id}"].Chats
    .Request()
    .GetAsync();

```