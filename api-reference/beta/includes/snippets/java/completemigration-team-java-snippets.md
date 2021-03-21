---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e96cf507dc3ebde97693c5cd968bbe0cbc41de34
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970088"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{teamId}")
    .completeMigration()
    .buildRequest()
    .post();

```