---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a998f61869ce664dff595963fd31456cfa7b59449ba7690e30cd793f67eef228
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278789"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.compliance().ediscovery().cases("061b9a92-8926-4bd9-b41d-abf35edc7583")
    .reopen()
    .buildRequest()
    .post();

```