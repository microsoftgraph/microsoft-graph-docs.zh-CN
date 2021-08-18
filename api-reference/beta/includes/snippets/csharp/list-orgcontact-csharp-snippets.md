---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 679868541a986915f9432e34e0026d015a2fd7677b0d15f6caffc84d1e5a83aa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218479"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contacts = await graphClient.Contacts
    .Request()
    .GetAsync();

```