---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85fe92c4abe28d4969640267b923c1008026079d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977632"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().permissionGrantPolicies("my-custom-consent-policy").excludes("6a846635-3e70-4a10-821e-512a0db93cbd")
    .buildRequest()
    .delete();

```