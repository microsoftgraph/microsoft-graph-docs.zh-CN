---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1f7eda1efeb0ca8578c3cc481497e7d398ec415
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972848"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.security().securityActions("{id}")
    .cancelSecurityAction()
    .buildRequest()
    .post();

```