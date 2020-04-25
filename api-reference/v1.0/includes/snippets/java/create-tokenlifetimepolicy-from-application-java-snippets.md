---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f63736492ea9fc69d5d7e3108b58fdfaa7e6b6e
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806725"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TokenLifetimePolicy tokenLifetimePolicy = new TokenLifetimePolicy();
tokenLifetimePolicy.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"));

graphClient.applications("{id}").tokenLifetimePolicies().references()
    .buildRequest()
    .post(tokenLifetimePolicy);

```