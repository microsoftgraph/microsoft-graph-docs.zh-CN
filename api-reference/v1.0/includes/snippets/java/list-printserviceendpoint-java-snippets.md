---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f3b04473ddbd85b95f4d621d348fa3f55eb0f0e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777017"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrintServiceEndpointCollectionPage endpoints = graphClient.print().services("{printServiceId}").endpoints()
    .buildRequest()
    .get();

```