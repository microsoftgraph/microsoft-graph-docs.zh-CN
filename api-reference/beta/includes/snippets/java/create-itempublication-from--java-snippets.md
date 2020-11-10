---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3e7bb57950e0e90a026cc7cb2c7e521ea48a4fc
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976259"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemPublication itemPublication = new ItemPublication();
itemPublication.description = "One persons journey to the top of the branding management field.";
itemPublication.displayName = "Got Brands? The story of Innocenty Popov and his journey to the top.";
itemPublication.publishedDate = new DateOnly(1900,1,1);
itemPublication.publisher = "International Association of Branding Management Publishing";
itemPublication.thumbnailUrl = "https://iabm.io/sdhdfhsdhshsd.jpg";
itemPublication.webUrl = "https://www.iabm.io";

graphClient.me().profile().publications()
    .buildRequest()
    .post(itemPublication);

```