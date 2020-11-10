---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c0b855567eec589fbc838176ed8528bfbd59f3c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981188"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{id}").claimsMappingPolicies("{id}").reference()
    .buildRequest()
    .delete();

```