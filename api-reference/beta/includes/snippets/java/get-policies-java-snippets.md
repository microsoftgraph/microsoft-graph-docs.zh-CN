---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46cef88642f08043ef7334ced159572e266a1054
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970601"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConditionalAccessPolicyCollectionPage policies = graphClient.identity().conditionalAccess().policies()
    .buildRequest()
    .filter("displayName eq 'SimplePolicy1' or displayName eq 'SimplePolicy2'")
    .get();

```