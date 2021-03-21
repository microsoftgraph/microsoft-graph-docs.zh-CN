---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a12c4d798ded192812778fcd88814aea0ed99372
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971178"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

HomeRealmDiscoveryPolicy homeRealmDiscoveryPolicy = graphClient.policies().homeRealmDiscoveryPolicies("{id}")
    .buildRequest()
    .get();

```