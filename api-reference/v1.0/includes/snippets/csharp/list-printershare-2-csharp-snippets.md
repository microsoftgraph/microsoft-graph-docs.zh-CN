---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b86b8be29f3fd32f2fa23954156f348f3a1704fc929538f67a884d4b49f83a6d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158408"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shares = await graphClient.Print.Printers["{printer-id}"].Shares
    .Request()
    .GetAsync();

```