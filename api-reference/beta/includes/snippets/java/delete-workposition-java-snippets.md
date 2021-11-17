---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e81ddb6520a023d649126a74190762ceb5ca07a0e85a7ab430311c9b0a8f584
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106846"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().positions("{id}")
    .buildRequest()
    .delete();

```