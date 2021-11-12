---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6aa945ae749f55319a7b7b6024ddb607ba5e1a6f4832eaffe09d37ba04b3ce25
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279467"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Shift shift = graphClient.teams("{teamId}").schedule().shifts("{shiftId}")
    .buildRequest()
    .get();

```