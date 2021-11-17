---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20f07b5da7ed839f6ed05143cebe29c4960fadae448ea1bc99727a18793ba2ae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104138"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstanceCollectionPage pendingAccessReviewInstances = graphClient.me().pendingAccessReviewInstances()
    .buildRequest()
    .expand("definition")
    .skip(0)
    .top(100)
    .get();

```