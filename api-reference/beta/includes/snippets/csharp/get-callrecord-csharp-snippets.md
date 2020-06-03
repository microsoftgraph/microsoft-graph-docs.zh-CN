---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5db6923a49454290f96e123da14ce81d28747ae5
ms.sourcegitcommit: 43f7800894857a29f02fffaf4a50ad6386b5bf59
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2020
ms.locfileid: "44524479"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var callRecord = await graphClient.Communications.CallRecords["{id}"]
    .Request()
    .GetAsync();

```