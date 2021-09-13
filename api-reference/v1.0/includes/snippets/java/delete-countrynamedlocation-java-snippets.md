---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 73f11a0d59efc3142da389f5932a7a3fe337a1b7f6229ba563ecebdc4faa9ebf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904145"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().conditionalAccess().namedLocations("1c4427fd-0885-4a3d-8b23-09a899ffa959")
    .buildRequest()
    .delete();

```