---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39cb91989e4d5c248c19b04cb69843d800d4bc96
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52668739"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var taughtClasses = await graphClient.Education.Classes["{educationClass-id}"].Members["{educationUser-id}"].TaughtClasses
    .Request()
    .GetAsync();

```