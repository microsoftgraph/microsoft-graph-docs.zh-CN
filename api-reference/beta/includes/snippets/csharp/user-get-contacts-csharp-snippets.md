---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7cd6384a1c56f7e15cb8d9cd40b5e14545da655ffa0745a3e2a5f884b0ed7ca6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333620"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contacts = await graphClient.Me.Contacts
    .Request()
    .Select("displayName,emailAddresses")
    .GetAsync();

```