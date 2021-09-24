---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bed6d31f34c31e97cefcbd2a5049704c84be9fdb120c9fdb2139bdc281b4bd53
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163706"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.devices("{id}")
    .buildRequest()
    .delete();

```