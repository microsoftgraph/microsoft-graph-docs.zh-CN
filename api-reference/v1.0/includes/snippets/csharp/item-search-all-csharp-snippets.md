---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ddb9d7ba2611de9bc6ed31151d002254f1225b9ffdda6c177ae2113e68c7dc0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903341"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var search = await graphClient.Me.Drive
    .Search("Contoso Project")
    .Request()
    .GetAsync();

```