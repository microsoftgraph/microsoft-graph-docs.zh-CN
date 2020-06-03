---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9417b4b77632ea2271ab723982e8f5df0106dbd2
ms.sourcegitcommit: 43f7800894857a29f02fffaf4a50ad6386b5bf59
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2020
ms.locfileid: "44524581"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sessions = await graphClient.Communications.CallRecords["{id}"].Sessions
    .Request()
    .Expand("segments")
    .GetAsync();

```