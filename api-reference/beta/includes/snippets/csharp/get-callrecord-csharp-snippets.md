---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e980d9983e2fc6829e20e8ddd3bbeb4586ef55cd7d3cadc13ead246bde643591
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903449"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var callRecord = await graphClient.Communications.CallRecords["{callRecords.callRecord-id}"]
    .Request()
    .GetAsync();

```