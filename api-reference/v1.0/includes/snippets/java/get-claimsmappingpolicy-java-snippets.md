---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47c680f428ab1514a97d0843166d8a1fb0f457c1
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863654"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ClaimsMappingPolicy claimsMappingPolicy = graphClient.policies().claimsMappingPolicies("{id}")
    .buildRequest()
    .get();

```