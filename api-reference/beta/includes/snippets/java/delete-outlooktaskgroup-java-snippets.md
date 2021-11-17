---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e95d67d224600bd647b0fd9ece5dad572d8938cbf87884fe8450e35fa15ceba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219732"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().outlook().taskGroups("AAMkADIyAAAhrbe-AAA=")
    .buildRequest()
    .delete();

```