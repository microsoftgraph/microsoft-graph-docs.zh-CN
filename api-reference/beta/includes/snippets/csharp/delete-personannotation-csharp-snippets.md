---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc850bccf826d0180df1b80b48a3bda3f1d485ffdc22f22c65cb55cb64b69e88
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164089"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Profile.Notes["{personAnnotation-id}"]
    .Request()
    .DeleteAsync();

```