---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 806f19371c3a4d975e0777af444d4264881b9762e6b7e5ed4931c8bad2693b86
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409690"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Printers["{printer-id}"].TaskTriggers["{printTaskTrigger-id}"]
    .Request()
    .DeleteAsync();

```