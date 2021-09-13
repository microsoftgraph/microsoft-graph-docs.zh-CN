---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e6c4eb0d2ee8eb38f8be7d0d78267cb2ff18fbe47f1f9674d04e0348e4b6415
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333471"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Subscription subscription = graphClient.me().drive().root().subscriptions("socketIo")
    .buildRequest()
    .get();

```