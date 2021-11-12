---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2412ef23511d711c952299fb37ab6eccf481170b993cac0eda01645ee49c1291
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162545"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printTaskTrigger = await graphClient.Print.Printers["{printer-id}"].TaskTriggers["{printTaskTrigger-id}"]
    .Request()
    .GetAsync();

```