---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b3daf72648110bf4e341c6cea2d03147ba5054905d07d1c3609ed423a2d3fd1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219006"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var profileCardProperties = await graphClient.Organization["{organization-id}"].Settings.ProfileCardProperties
    .Request()
    .GetAsync();

```