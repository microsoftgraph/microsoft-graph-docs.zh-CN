---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd83a7048bc1888fbf67c72e204c7d1ef7f23ef4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951662"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"].Members["{educationUser-id}"]
    .Request()
    .DeleteAsync();

```