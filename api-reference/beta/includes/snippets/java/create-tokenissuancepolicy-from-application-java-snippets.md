---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 954dad092c4accfe34244d0dada53786906b3f82
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961903"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TokenIssuancePolicy tokenIssuancePolicy = new TokenIssuancePolicy();
tokenIssuancePolicy.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/policies/tokenIssuancePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"));

graphClient.applications("{id}").tokenIssuancePolicies().references()
    .buildRequest()
    .post(tokenIssuancePolicy);

```