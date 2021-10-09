---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60a2d694d7039c28a88acab151b969e6ad119b5d5b9aa28da7d73aece8ecc4a3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105200"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryRoleTemplates = await graphClient.DirectoryRoleTemplates
    .Request()
    .GetAsync();

```