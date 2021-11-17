---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e1f1f387e9e98df69926d8818dc97651376f44ab462f39db47c0034ab9e3a4b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219647"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transitiveMemberOf = await graphClient.Groups["{group-id}"].TransitiveMemberOf
    .Request()
    .GetAsync();

```