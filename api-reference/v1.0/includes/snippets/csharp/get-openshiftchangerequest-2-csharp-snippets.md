---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 080c27b0d3cb6a57eca9103f88f52d15a09c27f042cd7126deda223d5c74f00f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409700"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var openShiftChangeRequests = await graphClient.Teams["{team-id}"].Schedule.OpenShiftChangeRequests
    .Request()
    .GetAsync();

```