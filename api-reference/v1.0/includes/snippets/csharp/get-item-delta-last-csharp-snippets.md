---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a5b5699d583f6b07c7f049baa393224b694056802c5094911ff2058b3de6aad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104603"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.Drive.Root
    .Delta("1230919asd190410jlka")
    .Request()
    .GetAsync();

```