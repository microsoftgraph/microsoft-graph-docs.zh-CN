---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aeb77115780e39dee15f310631ca9d02ce23b49989067846d0696dee6d53cefb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219886"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryRoleTemplate = await graphClient.DirectoryRoleTemplates["{directoryRoleTemplate-id}"]
    .Request()
    .GetAsync();

```