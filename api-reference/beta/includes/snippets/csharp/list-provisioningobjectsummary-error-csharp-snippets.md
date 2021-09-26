---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d64f7c5700d39c098488cbbb7be362b6568723ce84faf0eeb3290887094ab98
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163093"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var provisioning = await graphClient.AuditLogs.Provisioning
    .Request()
    .GetAsync();

```