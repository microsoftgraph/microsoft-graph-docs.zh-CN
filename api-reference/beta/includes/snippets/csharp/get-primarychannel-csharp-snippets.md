---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a8ff48e44a69e23e8f7a418ac2fb8d1c2ad0163119a6ab4edc5ed8a34f8bc87
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104475"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channel = await graphClient.Teams["{team-id}"].PrimaryChannel
    .Request()
    .GetAsync();

```