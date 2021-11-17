---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a3b9b62717d5dbacdec22bca86c13dad4d1455744da49201fc4ad28ee7a957f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105104"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserAccountInformation userAccountInformation = new UserAccountInformation();
userAccountInformation.countryCode = "NO";

graphClient.me().profile().account("{id}")
    .buildRequest()
    .patch(userAccountInformation);

```