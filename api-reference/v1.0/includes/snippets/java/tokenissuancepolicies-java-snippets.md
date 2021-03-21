---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f90fa8eddd51c126697adf610837b6421d701dc1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971082"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TokenIssuancePolicyCollectionPage tokenIssuancePolicies = graphClient.policies().tokenIssuancePolicies()
    .buildRequest()
    .get();

```