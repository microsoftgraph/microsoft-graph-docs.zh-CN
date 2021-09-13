---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7bc58363c841f9649433ab1dc8c196f5561316b1b98db6585790563c5af7a9c8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274448"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organizationalBrandingLocalization = await graphClient.Organization["{organization-id}"].Branding.Localizations["{organizationalBrandingLocalization-id}"]
    .Request()
    .GetAsync();

```