---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca5ef0e1b365d428701293471493a52134d13ab804dc7f6fe834474e852bea32
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221420"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groupSettings("{id}")
    .buildRequest()
    .delete();

```