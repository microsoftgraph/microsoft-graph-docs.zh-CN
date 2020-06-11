---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1bfa93349f675a1572ba1b7980b2704f890ef07b
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684935"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Me.Messages
    .Request()
    .Select("sender,subject")
    .GetAsync();

```