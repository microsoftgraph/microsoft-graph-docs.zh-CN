---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 857998e7436a60b334df607907785d17f1a7827bed98fc0e8b2bc8ced0d69f72
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902405"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var presence = await graphClient.Me.Presence
    .Request()
    .GetAsync();

```