---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 767cf260a8909660408f332165301875120b6f02a9136e03b8764e1bba5d571f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103791"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Users
    .Delta()
    .Request()
    .Select("displayName,jobTitle,mobilePhone")
    .GetAsync();

```