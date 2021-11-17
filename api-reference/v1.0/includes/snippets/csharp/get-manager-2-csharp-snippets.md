---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab61cda855cf9be160c3da0408fd995ca24553e2b4a553a01bbf3f3b39986d81
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409458"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.Users["{user-id}"].Manager
    .Request()
    .GetAsync();

```