---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e74a6f187628fb502ab5d33360d3a80f3394f739ee0715ca98d1e981898df97c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902645"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewPolicy accessReviewPolicy = graphClient.policies().accessReviewPolicy()
    .buildRequest()
    .get();

```