---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62d32b02497f9dcade6c4124bddaf35b797b6d0862e4a96480c0567f916ef853
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218463"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedApproval = await graphClient.PrivilegedApproval
    .Request()
    .GetAsync();

```