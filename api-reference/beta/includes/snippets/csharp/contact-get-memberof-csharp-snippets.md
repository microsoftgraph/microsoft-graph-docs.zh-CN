---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20924c0848ef35de447a82c339e3e17f0308cec1e22a8023559a96378e77a589
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902496"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberOf = await graphClient.Contacts["{orgContact-id}"].MemberOf
    .Request()
    .GetAsync();

```