---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f34c94ada62575c8ff2d95f0504dd1cdc2466a3cea5f6ea12f4dccabf7d145b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162166"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkPosition workPosition = new WorkPosition();
workPosition.isCurrent = true;

graphClient.me().profile().positions("{id}")
    .buildRequest()
    .patch(workPosition);

```