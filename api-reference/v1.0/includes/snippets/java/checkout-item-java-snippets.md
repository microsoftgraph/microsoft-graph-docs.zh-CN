---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d02f214da8755b69887d846da97e522b9f644cb8fe0b0f3edd7da2ce1f1beb4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106478"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.drives("{drive-id}").items("{item-id}")
    .checkout()
    .buildRequest()
    .post();

```