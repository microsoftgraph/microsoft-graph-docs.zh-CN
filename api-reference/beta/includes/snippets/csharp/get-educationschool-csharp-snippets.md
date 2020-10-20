---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07d042e281b4762a6498ec001dbd9bb9918fc650
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48622240"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSchool = await graphClient.Education.Schools["10001"]
    .Request()
    .GetAsync();

```