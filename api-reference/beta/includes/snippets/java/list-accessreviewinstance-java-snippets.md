---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6c856bc5a0f2b187af3a210fcf1c2b98e055487511f26b091f3fc2a92a87e4c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902678"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstanceCollectionPage instances = graphClient.identityGovernance().accessReviews().definitions("8564a649-4f67-4e09-88e7-55def6530e88").instances()
    .buildRequest()
    .skip(0)
    .top(100)
    .get();

```