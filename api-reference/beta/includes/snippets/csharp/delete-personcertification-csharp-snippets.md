---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3cc78702b6cba566f9ac8ee5868bc9db8ba9edfebf6de152150c75d99cb9ac60
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328763"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Profile.Certifications["{personCertification-id}"]
    .Request()
    .DeleteAsync();

```