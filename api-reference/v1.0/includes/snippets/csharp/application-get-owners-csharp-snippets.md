---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7bbfc6ab83989004f1f4c8a6a198f5616228182f7c15d264521cac9ea9a01d8b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161810"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var owners = await graphClient.Applications["{application-id}"].Owners
    .Request()
    .GetAsync();

```