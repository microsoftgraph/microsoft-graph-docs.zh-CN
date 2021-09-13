---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76a9931ac52f76ae4d6c7be70d8c0dfdc03360db8489d37429c7e132c63b40f3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903900"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drives["{drive-id}"].Items["{driveItem-id}"]
    .Checkout()
    .Request()
    .PostAsync();

```