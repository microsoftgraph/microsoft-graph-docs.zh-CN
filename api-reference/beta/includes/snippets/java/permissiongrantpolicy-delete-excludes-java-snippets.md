---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ae66fd5a184defc59f6757e19abd18e00296d3ec21819bfcdb11a92225271ce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221232"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().permissionGrantPolicies("my-custom-consent-policy").excludes("6a846635-3e70-4a10-821e-512a0db93cbd")
    .buildRequest()
    .delete();

```