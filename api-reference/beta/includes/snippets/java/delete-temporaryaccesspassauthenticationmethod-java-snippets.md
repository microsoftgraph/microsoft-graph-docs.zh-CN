---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e79d1878a43856f3671ed26054f5b39c2e1406e11c8314782cf1a579dfbcc04e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378604"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("kim@contoso.com").authentication().temporaryAccessPassMethods("{id}")
    .buildRequest()
    .delete();

```