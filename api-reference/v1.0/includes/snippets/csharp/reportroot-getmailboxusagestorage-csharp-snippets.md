---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7051e54464b8b3ee0beb1985869af8b56598256d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327201"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetMailboxUsageStorage("D7")
    .Request()
    .GetAsync();

```