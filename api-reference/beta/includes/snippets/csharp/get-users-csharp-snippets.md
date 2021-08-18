---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60b41c542f941e07a87ef0e6fb404aad12e4e99ac394a54c1a40b3c30e859ab0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378554"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users
    .Request()
    .GetAsync();

```