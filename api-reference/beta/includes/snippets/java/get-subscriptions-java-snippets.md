---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51b7679c6222227c510d57512c5f538b3d33e8d1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982252"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SubscriptionCollectionPage subscriptions = graphClient.subscriptions()
    .buildRequest()
    .get();

```