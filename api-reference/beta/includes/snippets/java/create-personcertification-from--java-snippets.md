---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6feaafbfc5d6e46879e74912ca38fa3217fb57ad
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968753"
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