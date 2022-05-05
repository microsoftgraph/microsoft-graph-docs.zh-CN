---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42e810d79fb6045f343293f0968a6a4a158ebea9
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220339"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SignInCollectionPage signIns = graphClient.auditLogs().signIns()
    .buildRequest()
    .filter("startsWith(appDisplayName,'Graph')")
    .top(10)
    .get();

```