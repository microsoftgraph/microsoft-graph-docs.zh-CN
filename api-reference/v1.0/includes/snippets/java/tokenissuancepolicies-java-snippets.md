---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e5341184494d94ad572968b03c89fafc35a5f3d00e42724c7815523736fa30b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104925"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TokenIssuancePolicyCollectionPage tokenIssuancePolicies = graphClient.policies().tokenIssuancePolicies()
    .buildRequest()
    .get();

```