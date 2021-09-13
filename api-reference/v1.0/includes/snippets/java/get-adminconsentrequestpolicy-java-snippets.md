---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be9c3878ed20eab3be7a4183a2c9ae272b6464ccf76fc783144a84b60ee75d52
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378814"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AdminConsentRequestPolicy adminConsentRequestPolicy = graphClient.policies().adminConsentRequestPolicy()
    .buildRequest()
    .get();

```