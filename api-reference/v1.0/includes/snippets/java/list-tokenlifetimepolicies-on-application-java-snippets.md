---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa54af4a07923ff200ca08c6c10515a17358234e
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43771080"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITokenLifetimePolicyCollectionPage tokenLifetimePolicies = graphClient.applications("{id}").tokenLifetimePolicies()
    .buildRequest()
    .get();

```