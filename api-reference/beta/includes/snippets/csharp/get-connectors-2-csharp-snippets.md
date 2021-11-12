---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8b3a3e37c3186c54441c57c0a9caad521af560eea3b6d0a02e5de2c36a43753
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220081"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectors = await graphClient.Print.Connectors
    .Request()
    .GetAsync();

```