---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 049fa97f53fae6504dc9b2dd6aefd48d64cc2bd5
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471028"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IGroupCollectionPage groups = graphClient.groups()
    .buildRequest()
    .filter("membershipRuleProcessingState eq 'On'")
    .select("id,membershipRule,membershipRuleProcessingState,membershipRuleProcessingStatus")
    .get();

```