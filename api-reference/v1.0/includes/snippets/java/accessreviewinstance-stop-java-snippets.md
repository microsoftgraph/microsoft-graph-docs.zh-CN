---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ffda1c9b4a703951a5d61f6c909c6400c45c9420
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211027"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().accessReviews().definitions("8564a649-4f67-4e09-88e7-55def6530e88").instances("1234a649-4f67-1234-88e7-55def6530e88")
    .stop()
    .buildRequest()
    .post();

```