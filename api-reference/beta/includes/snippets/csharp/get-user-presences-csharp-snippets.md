---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8a48c173b65de24683f6f42209ccff2b0e571b0
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863335"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var presence = await graphClient.Communications.Presences["dc74d9bb-6afe-433d-8eaa-e39d80d3a647"]
    .Request()
    .GetAsync();

```