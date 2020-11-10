---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56941ef2f1ee8c5a8f2e936ef063e52609d6814f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969609"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String id = "5793aa3b-cca9-4794-679a240f8b58";

graphClient.servicePrincipals("{id}")
    .deletePasswordSingleSignOnCredentials(id)
    .buildRequest()
    .post();

```