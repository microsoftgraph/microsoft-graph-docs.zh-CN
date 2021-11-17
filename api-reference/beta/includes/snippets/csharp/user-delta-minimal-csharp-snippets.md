---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36815466af1b7d267da3d26c93b3afbed4ed7ec2de47b3ca2590d8e8554622d8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902462"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Users
    .Delta()
    .Request()
    .Header("Prefer","return=minimal")
    .Select("displayName,jobTitle,mobilePhone")
    .GetAsync();

```