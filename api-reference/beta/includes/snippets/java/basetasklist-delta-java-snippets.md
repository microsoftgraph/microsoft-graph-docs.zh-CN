---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2038051fb74011d9e06c021e8c2708c5d5ecff3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094874"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BaseTaskListDeltaCollectionPage delta = graphClient.me().tasks().lists()
    .delta()
    .buildRequest()
    .get();

```