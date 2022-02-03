---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef189aa432a669c51789164dc14ff329f9d1e11d
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351803"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("19c308f2-e088-464d-8ccb-7137b7bab660").homeRealmDiscoveryPolicies("6c6f154f-cb39-4ff9-bf5b-62d5ad585cde").reference()
    .buildRequest()
    .delete();

```