---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aea9f056d7015109e9ec5d5b02d19927cf2f6e61f42d51b71392c75a869e8be6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333135"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"].Members["{educationUser-id}"]
    .Request()
    .DeleteAsync();

```