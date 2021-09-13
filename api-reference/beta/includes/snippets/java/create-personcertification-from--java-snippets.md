---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0523ef78cd3279ec20daee0054655513107d46a1855eb9fa2ee690521d69b350
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278923"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonCertification personCertification = new PersonCertification();
personCertification.certificationId = "KB-1235466333663322";
personCertification.description = "Blackbelt in Marketing - Brand Management";
personCertification.displayName = "Marketing Blackbelt - Brand Management";
personCertification.thumbnailUrl = "https://iame.io/dfhdfdfd334.jpg";
personCertification.webUrl = "https://www.iame.io/blackbelt";

graphClient.me().profile().certifications()
    .buildRequest()
    .post(personCertification);

```