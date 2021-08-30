---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6e5dc319b33e483fc21202273e4480b2517a18b7d151d3b5d2d386399ca329a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277394"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var findRooms = await graphClient.Me
    .FindRooms()
    .Request()
    .GetAsync();

```