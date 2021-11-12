---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ef5fe2baab5ace5cc1083ea575b7f39836729997fe8fe3aa8c6a61c7459a22e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162987"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberOf = await graphClient.Groups["{group-id}"].MemberOf
    .Request()
    .GetAsync();

```