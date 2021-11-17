---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd3faf6a6c145db81978a9a9a6a9eed53ca61f9918f7e7307e2407e87c77884d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220784"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.ServicePrincipals
    .Delta()
    .Request()
    .GetAsync();

```