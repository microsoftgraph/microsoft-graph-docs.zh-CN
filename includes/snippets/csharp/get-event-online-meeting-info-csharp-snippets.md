---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61338f6fa4c05d62774c316576adb2192963fa45
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44685111"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = await graphClient.Me.Events["AAMkADAGu0AABIGYDZAAA="]
    .Request()
    .Select("isOnlineMeeting,onlineMeetingProvider,onlineMeeting")
    .GetAsync();

```