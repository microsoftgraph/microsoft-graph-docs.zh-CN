---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db4cf277761e89a44f46768617116ea543d616455a77d7af9d5a210331886274
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103966"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getCredentialUserRegistrationCount = await graphClient.Reports
    .GetCredentialUserRegistrationCount()
    .Request()
    .GetAsync();

```