---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92d49d43afaf405fcb8d5fca1c3ecf5594d0798cae87ec74b0b39e3d5a4caf91
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902976"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"].Teachers["{educationUser-id}"]
    .Request()
    .DeleteAsync();

```