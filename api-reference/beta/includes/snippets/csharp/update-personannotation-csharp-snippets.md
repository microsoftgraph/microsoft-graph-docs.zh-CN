---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0d2b5313bfea8ef27ea8c7bc5b66807103f411d40a52a76f236034c2cffe3ca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220257"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personAnnotation = new PersonAnnotation
{
    AllowedAudiences = AllowedAudiences.Organization
};

await graphClient.Users["{user-id}"].Profile.Notes["{personAnnotation-id}"]
    .Request()
    .UpdateAsync(personAnnotation);

```