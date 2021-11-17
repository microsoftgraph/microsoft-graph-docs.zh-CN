---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab5a133609e14ba64ba03438e2ab461f111f4ada6e751efe9d54e87b7e56fa16
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220624"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Contacts
    .Delta()
    .Request()
    .GetAsync();

```