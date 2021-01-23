---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e959d20228461b2a041ef3598178521af9cfd841
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49944944"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectors = await graphClient.Print.Connectors
    .Request()
    .GetAsync();

```