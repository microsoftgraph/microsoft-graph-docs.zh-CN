---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: daf661fbffce27284d0fa204201b0059c15938b21d2b66f0b8304cba2b10693c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146199"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Me.Drive.Items["{item-id}"]
    .Request()
    .GetAsync();

```