---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80167eff13decde8d896a85ee96d21426a90d92e899b9e68db785e20bbd9ebd0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104393"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupCollectionPage groups = graphClient.groups()
    .buildRequest()
    .filter("membershipRuleProcessingState eq 'On'")
    .select("id,membershipRule,membershipRuleProcessingState,membershipRuleProcessingStatus")
    .get();

```