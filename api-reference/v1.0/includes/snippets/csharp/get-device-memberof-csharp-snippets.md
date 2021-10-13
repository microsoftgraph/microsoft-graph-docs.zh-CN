---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1cd008ca98521d0e117a231d27d876487c2a3c323d4a0d0a43f008d744cc5cc5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221435"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberOf = await graphClient.Devices["{device-id}"].MemberOf
    .Request()
    .GetAsync();

```