---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ebe41efae55ca87bdcf8968536c6d14d36163d123c2e2fbe918137700396071
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161859"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personAnnualEvent = new PersonAnnualEvent
{
    AllowedAudiences = AllowedAudiences.Contacts
};

await graphClient.Me.Profile.Anniversaries["{personAnnualEvent-id}"]
    .Request()
    .UpdateAsync(personAnnualEvent);

```