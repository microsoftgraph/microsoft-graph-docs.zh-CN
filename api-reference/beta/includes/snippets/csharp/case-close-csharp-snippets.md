---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6614e67028afe8e75e93b1d67e530d131f382dc1c420cce9b940caacc409c468
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218575"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"]
    .Close()
    .Request()
    .PostAsync();

```