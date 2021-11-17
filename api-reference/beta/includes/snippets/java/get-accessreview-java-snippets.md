---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2cad54edfe1757c1c351d24abae3b06c3b6eafa6353c73d5158c77da953ea2b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902731"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReview accessReview = graphClient.accessReviews("2b83cc42-09db-46f6-8c6e-16fec466a82d")
    .buildRequest()
    .get();

```