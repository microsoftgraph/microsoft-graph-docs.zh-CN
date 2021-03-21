---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 000fa1008efe9091edbf5b501426ca819d3ae81a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968481"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserAccountInformation userAccountInformation = new UserAccountInformation();
userAccountInformation.countryCode = "NO";

graphClient.me().profile().account("{id}")
    .buildRequest()
    .patch(userAccountInformation);

```