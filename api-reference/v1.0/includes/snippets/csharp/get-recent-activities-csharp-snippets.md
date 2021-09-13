---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c1fa94f0dc81c4f9813d7f9ec22514342689a9b7311247e346144fdf6c97cfb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221153"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var recent = await graphClient.Me.Activities
    .Recent()
    .Request()
    .GetAsync();

```