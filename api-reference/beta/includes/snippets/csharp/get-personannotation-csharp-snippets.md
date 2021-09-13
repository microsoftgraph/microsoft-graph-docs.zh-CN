---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66180589a8cf63a03f4419a5158cb67ba0fe786a74cdc234d9f00aa9ba18119f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219438"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personAnnotation = await graphClient.Me.Profile.Notes["{personAnnotation-id}"]
    .Request()
    .GetAsync();

```