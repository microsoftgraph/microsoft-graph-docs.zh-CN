---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ac2c0ac341e4f29263d505d71449fba9ca16cbe670bdf45404e936ad5fc99d2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220862"
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