---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9977c8a7b5116de772edac1c187558a838722197
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137745"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Education.Classes["{educationClass-id}"].AssignmentCategories
    .Delta()
    .Request()
    .GetAsync();

```