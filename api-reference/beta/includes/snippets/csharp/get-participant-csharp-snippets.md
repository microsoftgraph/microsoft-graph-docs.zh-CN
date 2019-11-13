---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6332fae7397b6dbb1a478113cde8bbe27d4a74cc
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38303058"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var participant = await graphClient.Communications.Calls["7531d31f-d10d-44de-802f-c569dbca451c"].Participants["7e1b4346-85a6-4bdd-abe3-d11c5d420efe"]
    .Request()
    .GetAsync();

```