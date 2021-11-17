---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ab41443c6105ddbd21bf876461020e3482f3367f21563a87cade8e52c3c2334
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105196"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Settings["{directorySetting-id}"]
    .Request()
    .DeleteAsync();

```