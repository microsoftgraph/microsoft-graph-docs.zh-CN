---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9583e169823e0c8c8418e1fbba1a846f9e7a4fec7d7c9f3f846b120fc93d10fa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57331874"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TodoTaskList todoTaskList = new TodoTaskList();
todoTaskList.displayName = "Vacation Plan";

graphClient.me().todo().lists("AAMkADIyAAAhrbPWAAA=")
    .buildRequest()
    .patch(todoTaskList);

```