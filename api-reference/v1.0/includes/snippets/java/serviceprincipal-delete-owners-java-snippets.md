---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ee0da70b0ff676ce199236cfb96caf586cdcb8e258a52ae0aad6c17fb73d453
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57408976"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{id}").owners("{id}").reference()
    .buildRequest()
    .delete();

```