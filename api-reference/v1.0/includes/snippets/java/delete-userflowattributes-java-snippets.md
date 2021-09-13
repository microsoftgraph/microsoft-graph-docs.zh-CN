---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 551c09dcc545104ff61d0e507bbc6e576ea49e364c1049016cdcddefe2cf88c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161619"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().userFlowAttributes("extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby")
    .buildRequest()
    .delete();

```