---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7395c8b0cbdf3130b9119e7025e653dc486956f93cb7e483251ff8fd0292af12
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903277"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TrustFrameworkKeySetCollectionPage keySets = graphClient.trustFramework().keySets()
    .buildRequest()
    .get();

```