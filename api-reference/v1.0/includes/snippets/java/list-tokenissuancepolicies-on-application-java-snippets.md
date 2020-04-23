---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70b7375506fd22f8d3c8481efb22539d15abc612
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43770976"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITokenIssuancePolicyCollectionPage tokenIssuancePolicies = graphClient.applications("{id}").tokenIssuancePolicies()
    .buildRequest()
    .get();

```