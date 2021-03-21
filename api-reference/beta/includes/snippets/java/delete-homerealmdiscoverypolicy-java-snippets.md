---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4015bec7a3923376ee39a209c96466697e8818a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979509"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().homeRealmDiscoveryPolicies("{id}")
    .buildRequest()
    .delete();

```