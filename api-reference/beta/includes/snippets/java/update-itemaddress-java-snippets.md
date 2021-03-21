---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c840ded07e5a4186cb16f5c9ec09d1fef6681155
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981853"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemAddress itemAddress = new ItemAddress();
itemAddress.allowedAudiences = EnumSet.of(AllowedAudiences.ME);
itemAddress.displayName = "Secret Hideout";

graphClient.users("{userId}").profile().addresses("{id}")
    .buildRequest()
    .patch(itemAddress);

```