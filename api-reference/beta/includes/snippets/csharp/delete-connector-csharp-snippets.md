---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6016b77b4ae3379a7aa5921c5dd6d21dac417633
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793219"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Connectors["{printConnector-id}"]
    .Request()
    .DeleteAsync();

```