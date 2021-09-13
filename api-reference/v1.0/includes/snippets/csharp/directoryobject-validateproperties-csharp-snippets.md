---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0d879a320d89bfb261a9a57f63989701f971f6f246eb898a5aa10bae1999e4d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104607"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var entityType = "Group";

var displayName = "Myprefix_test_mysuffix";

var mailNickname = "Myprefix_test_mysuffix";

var onBehalfOfUserId = Guid.Parse("onBehalfOfUserId-value");

await graphClient.DirectoryObjects
    .ValidateProperties(entityType,displayName,mailNickname,onBehalfOfUserId)
    .Request()
    .PostAsync();

```