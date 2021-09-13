---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b0c93a990bdc659eca36849d3bcfbbe32efd611cee53717b3b462a029ae6f65
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105000"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationClass = await graphClient.Education.Classes["{educationClass-id}"]
    .Request()
    .GetAsync();

```