---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e499dc571d8522651ef7f5772d53abbe888cb37188aefa849c115c7905008cf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101360"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().shares("{id}").allowedGroups("{id}").reference()
    .buildRequest()
    .delete();

```