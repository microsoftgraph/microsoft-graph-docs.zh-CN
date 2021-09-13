---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0bac7777ff4981c4d6933b14664417b098901e95740b11c7930709b2b7da0216
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162798"
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