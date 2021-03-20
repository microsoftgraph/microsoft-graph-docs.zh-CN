---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3fc7e9cb9d6b6e7f367e5911a8775c6fbff44e09
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956320"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectors = await graphClient.Print.Printers["{printer-id}"].Connectors
    .Request()
    .GetAsync();

```