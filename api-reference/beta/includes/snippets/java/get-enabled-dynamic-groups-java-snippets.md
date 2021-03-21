---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2acb983d5a2ecd2916f1b77274df29ff8411db4e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980270"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupCollectionPage groups = graphClient.groups()
    .buildRequest()
    .filter("membershipRuleProcessingState eq 'On'")
    .select("id,membershipRule,membershipRuleProcessingState,membershipRuleProcessingStatus")
    .get();

```