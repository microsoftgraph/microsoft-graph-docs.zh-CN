---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6be5c2747da2a1ad8aaa54ced790b2ae38a92ddc81fcfccc4369fc9b1912a6e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107149"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.DirectoryRoles
    .Delta()
    .Request()
    .GetAsync();

```