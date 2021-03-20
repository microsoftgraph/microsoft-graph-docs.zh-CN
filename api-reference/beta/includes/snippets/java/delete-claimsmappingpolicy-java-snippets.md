---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90c4167e5cdfe07d38319b07f7de6e44fb5bef04
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976189"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().claimsMappingPolicies("{id}")
    .buildRequest()
    .delete();

```