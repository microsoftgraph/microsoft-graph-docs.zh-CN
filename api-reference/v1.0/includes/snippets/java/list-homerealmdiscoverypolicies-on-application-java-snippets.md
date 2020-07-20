---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ce143f7dd0c05b54a3534e3e66032161fdb5e5c
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863582"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IHomeRealmDiscoveryPolicyCollectionPage homeRealmDiscoveryPolicies = graphClient.servicePrincipals("{id}").homeRealmDiscoveryPolicies()
    .buildRequest()
    .get();

```