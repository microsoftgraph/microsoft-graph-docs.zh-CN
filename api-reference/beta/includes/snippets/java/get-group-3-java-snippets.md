---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c33828f63b5ace4d2c7a6eb666b7c0109aae59eb
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580298"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = graphClient.termStore().groups("1FFD3F87-9464-488A-A0EC-8FB90911182C")
    .buildRequest()
    .get();

```