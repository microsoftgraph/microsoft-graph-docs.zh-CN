---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cb7efbfde84e140fe8d3b5f381f351e51a0d2a803cb2860ecf07b06d8f23c17
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278333"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var supportedTimeZones = await graphClient.Me.Outlook
    .SupportedTimeZones(TimeZoneStandard.Iana)
    .Request()
    .GetAsync();

```