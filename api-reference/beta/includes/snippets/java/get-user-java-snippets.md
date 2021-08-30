---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 608e14016c5f62497c563b854150af835ecfb2ec8ea2ac64365d3b182ae494ba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218835"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = graphClient.me()
    .buildRequest()
    .get();

```