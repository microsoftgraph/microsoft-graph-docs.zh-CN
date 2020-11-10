---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2c000d3e479ecfc956eca60e6efb1744cb350ba
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964542"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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