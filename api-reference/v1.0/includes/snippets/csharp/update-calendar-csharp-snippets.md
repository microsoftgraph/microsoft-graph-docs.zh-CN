---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9cfb6b4ca2a1c03904bf376c286dc238327e012e6d053a72036f52895adc7df
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215752"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendar = new Calendar
{
    Name = "Social events"
};

await graphClient.Me.Calendar
    .Request()
    .UpdateAsync(calendar);

```