---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d921a2a6aa1b609030408f5b45da6095303cbe9bc80eb1de87fa7a5e270814aa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129766"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = graphClient.me().messages("AAMkADI4oeRpAABf0HJUAAA=")
    .buildRequest()
    .get();

```