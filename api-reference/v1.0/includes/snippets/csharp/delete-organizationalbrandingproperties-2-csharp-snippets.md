---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad5b96df378ad35335fd8106140f41fd3c3a9a5d7e5267bca81a72406cbafec6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162021"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Organization["{organization-id}"].Branding.Localizations["{organizationalBrandingLocalization-id}"]
    .Request()
    .DeleteAsync();

```