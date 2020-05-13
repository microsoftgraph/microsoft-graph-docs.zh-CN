---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35cd74713352c3d803407d90248af0eeaeebbd2b
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "43510609"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Administrativeunits
    .Delta()
    .Request()
    .GetAsync();

```