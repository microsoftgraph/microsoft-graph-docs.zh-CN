---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b885aed27a4dd9b4903c5c53373cc18d707e5cf70a0457f65c5bae766ae2c2b2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903291"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var serviceUpdateMessage = await graphClient.Admin.ServiceAnnouncement.Messages["{serviceUpdateMessage-id}"]
    .Request()
    .GetAsync();

```