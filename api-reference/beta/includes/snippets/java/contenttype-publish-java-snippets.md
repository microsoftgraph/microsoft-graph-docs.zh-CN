---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ccf6f60d374e1609a4217097f212a234e785689
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770440"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.sites("{siteId}").contentTypes("{contentTypeId}")
    .publish()
    .buildRequest()
    .post();

```