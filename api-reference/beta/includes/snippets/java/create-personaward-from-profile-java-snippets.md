---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d3247ca4e5b7ded4e8e3cfacc302d9ba84bdc52
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971745"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonAward personAward = new PersonAward();
personAward.description = "Lifetime Achievement award from the International Association of Branding Managers";
personAward.displayName = "Lifetime Achievement Award For Excellence in Branding";
personAward.issuedDate = new DateOnly(1900,1,1);
personAward.issuingAuthority = "International Association of Branding Management";
personAward.thumbnailUrl = "https://iabm.io/sdhdfhsdhshsd.jpg";
personAward.webUrl = "https://www.iabm.io";

graphClient.me().profile().awards()
    .buildRequest()
    .post(personAward);

```