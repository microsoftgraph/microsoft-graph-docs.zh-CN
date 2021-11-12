---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2afa43de0b4839aba5f01462aae58d6bb339d6e655a81f79e3ea350e9363f192
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105558"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupLifecyclePolicy groupLifecyclePolicy = graphClient.groupLifecyclePolicies("{id}")
    .buildRequest()
    .get();

```