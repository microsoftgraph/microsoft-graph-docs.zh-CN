---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 32a03cb85790329d169abd438eb8d391fd6a76aa003ea100728e3dc03900ddc8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903806"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Education.Classes["{educationClass-id}"].Members
    .Request()
    .GetAsync();

```