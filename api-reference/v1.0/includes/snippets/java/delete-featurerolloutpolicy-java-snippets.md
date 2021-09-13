---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b1fbffb6e86bef7c52a1f329c9ce279f7498614713a6dbc52098f8f991300db
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332436"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().featureRolloutPolicies("df85e4d9-e8c4-4033-a41c-73419a95c29c")
    .buildRequest()
    .delete();

```