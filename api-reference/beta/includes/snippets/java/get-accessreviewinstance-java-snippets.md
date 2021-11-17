---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99d852137a5047bab54e2c2e015981e3339e46e567244f5172909116ce24b86a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902680"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstance accessReviewInstance = graphClient.identityGovernance().accessReviews().definitions("6af553ce-104d-4842-ab5f-67d7b556e9dd").instances("9ea56d3c-8746-4cdf-9ccc-c7fe1a267c24")
    .buildRequest()
    .get();

```