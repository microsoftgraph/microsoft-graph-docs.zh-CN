---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85d6c2419ccd456357080ae8ac6e03e5e6a11b2a
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791176"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var regionalAndLanguageSettings = await graphClient.Me.Settings.RegionalAndLanguageSettings
    .Request()
    .GetAsync();

```