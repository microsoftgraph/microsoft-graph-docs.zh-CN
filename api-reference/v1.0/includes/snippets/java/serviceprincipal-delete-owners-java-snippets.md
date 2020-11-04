---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72df4b83ac3549bef5847dc92cb4abba7852a093
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903506"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{id}").owners("{id}").reference()
    .buildRequest()
    .delete();

```