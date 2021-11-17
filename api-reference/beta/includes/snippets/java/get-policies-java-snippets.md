---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15518a02ab272824cca77ab7c96c84122d6d0479494dc62cf90baa91f7fe91d4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278136"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConditionalAccessPolicyCollectionPage policies = graphClient.identity().conditionalAccess().policies()
    .buildRequest()
    .filter("displayName eq 'SimplePolicy1' or displayName eq 'SimplePolicy2'")
    .get();

```