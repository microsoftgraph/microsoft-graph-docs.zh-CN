---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 38f18d04dfefe069f54abba7eaf0e1cac9f247a227ce83164e9f9dd7bf5ba083
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54240515"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = await graphClient.Me.Events["AAMkADAGu0AABIGYDZAAA="]
    .Request()
    .Select("isOnlineMeeting,onlineMeetingProvider,onlineMeeting")
    .GetAsync();

```