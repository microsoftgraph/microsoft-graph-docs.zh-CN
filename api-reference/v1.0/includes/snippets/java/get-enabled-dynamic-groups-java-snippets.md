---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9cd4d455639ebcbd4fc602f4ae998adb138f533
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996078"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

GroupCollectionPage groups = graphClient.groups()
    .buildRequest( requestOptions )
    .filter("mailEnabled eq false and securityEnabled eq true and NOT(groupTypes/any(s:s eq 'Unified')) and membershipRuleProcessingState eq 'On'")
    .select("id,membershipRule,membershipRuleProcessingState")
    .get();

```