---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3fa80cccf5bd67e535dec4fc9ee8dcd5c73f0f80
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904970"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().todo().lists("AAMkADIyAAAhrbPXAAA=")
    .buildRequest()
    .delete();

```