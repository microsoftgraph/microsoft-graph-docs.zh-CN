---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ecf61ea0b747f0e3bf0b371fd7beb5f8492e9b4e5a0cb45b00db24cd05a12a2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163965"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Schedule.OpenShifts["{openShift-id}"]
    .Request()
    .DeleteAsync();

```