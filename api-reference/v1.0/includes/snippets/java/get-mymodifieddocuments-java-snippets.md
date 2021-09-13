---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dfb995acffb4eb0ae0f671b35d875fd611d6ea587b8a3ceb0501a0f3ac5df3dc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107017"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UsedInsightCollectionPage used = graphClient.me().insights().used()
    .buildRequest()
    .get();

```