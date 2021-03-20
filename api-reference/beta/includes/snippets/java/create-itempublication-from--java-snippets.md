---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e6f0a4b1887ca1c7588a44aedd5958cc240676f6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967271"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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