---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68773952b7bb502e030278674e68aaf2114ca07678300a6797b937f08a2a946f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902387"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Printers["{printer-id}"]
    .RestoreFactoryDefaults()
    .Request()
    .PostAsync();

```