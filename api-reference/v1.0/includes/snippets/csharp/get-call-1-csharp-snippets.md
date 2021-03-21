---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34de61c71074a436076fdfe4b279f3c9bc187e05
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964494"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var call = await graphClient.Communications.Calls["{call-id}"]
    .Request()
    .GetAsync();

```