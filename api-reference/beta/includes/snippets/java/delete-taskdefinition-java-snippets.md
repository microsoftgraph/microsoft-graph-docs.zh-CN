---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78c0ab0a10bf301b7cc80f51ec3968fe42867e19823abc5ffa7c6e9ee013228d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903394"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().taskDefinitions("4c6a0f26-8e5d-4bf6-91e6-4a5731adec19")
    .buildRequest()
    .delete();

```