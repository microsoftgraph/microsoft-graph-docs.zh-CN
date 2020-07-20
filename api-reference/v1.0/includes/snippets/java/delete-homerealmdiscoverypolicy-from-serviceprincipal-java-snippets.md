---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 099b3f15390a14c854adc36060cd6ad111f52ccd
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864115"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{id}").homeRealmDiscoveryPolicies("{id}").reference()
    .buildRequest()
    .delete();

```