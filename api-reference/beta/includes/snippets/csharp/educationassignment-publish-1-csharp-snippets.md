---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19587daf92968113bd5a0fb0808b01075f833361
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951826"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @string = await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"]
    .GetResourcesFolderUrl()
    .Request()
    .GetAsync();

```