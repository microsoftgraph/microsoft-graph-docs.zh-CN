---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af26fa37bdf7f412b1e638b9137fdb0a273a32224dc9c3f26e0a46c882f91f99
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164189"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Contacts
    .Delta()
    .Request()
    .Select("displayName,jobTitle,mail")
    .GetAsync();

```