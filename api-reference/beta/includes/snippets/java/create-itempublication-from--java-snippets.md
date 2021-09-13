---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03b073f15ef6fdaa5e8e929abe51762601bbe4da19cbb8276e2191869ef0a46d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164081"
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