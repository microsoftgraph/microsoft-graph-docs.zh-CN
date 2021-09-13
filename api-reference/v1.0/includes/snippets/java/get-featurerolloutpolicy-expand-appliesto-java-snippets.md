---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3e55360acdd2e3de8295a76f10ba4db707feb8ad44b82d4480b299952ec7ad5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221179"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

FeatureRolloutPolicy featureRolloutPolicy = graphClient.policies().featureRolloutPolicies("df85e4d9-e8c4-4033-a41c-73419a95c29c")
    .buildRequest()
    .expand("appliesTo")
    .get();

```