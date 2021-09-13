---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 999b26cae99638239c7e88d731a9722e441ac6cf9674c8beafcb8ff979f0018e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329090"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"]
    .Request()
    .DeleteAsync();

```