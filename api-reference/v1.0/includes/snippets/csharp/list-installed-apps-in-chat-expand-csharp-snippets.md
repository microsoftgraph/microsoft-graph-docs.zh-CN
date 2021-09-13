---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7cee08a3fa5cc7d6a3df00db5e0bd122ce74b635d420de0658ba178c2b5dc495
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904164"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Chats["{chat-id}"].InstalledApps
    .Request()
    .Expand("teamsAppDefinition($expand=bot)")
    .GetAsync();

```