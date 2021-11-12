---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9317774d5ae7e9f0564b75c0c24e72a7991522b9a0f1929b476f063358b30f6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328935"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.ContactFolders["{contactFolder-id}"].Contacts
    .Delta()
    .Request()
    .Select("displayName")
    .GetAsync();

```