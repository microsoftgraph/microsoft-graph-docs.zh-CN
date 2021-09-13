---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 209b8042dc42c3c86fd9faab251cad68f4e2984b514c67f5bac9920a8a6bfc11
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333190"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemPublication itemPublication = new ItemPublication();
itemPublication.publisher = "International Association of Branding Management Publishing";
itemPublication.thumbnailUrl = "https://iabm.io/sdhdfhsdhshsd.jpg";

graphClient.users("{userId}").profile().publications("{id}")
    .buildRequest()
    .patch(itemPublication);

```