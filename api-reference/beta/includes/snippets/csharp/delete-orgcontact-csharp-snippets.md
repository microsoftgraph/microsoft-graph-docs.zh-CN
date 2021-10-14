---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a06ab0ab3263a1ef5f4dcc995efc2266df4a3d08d0cdb4218a3e7a733a916950
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161201"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Contacts["{orgContact-id}"]
    .Request()
    .DeleteAsync();

```