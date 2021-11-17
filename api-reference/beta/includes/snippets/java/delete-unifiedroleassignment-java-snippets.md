---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64c6bf887a25b453470aadf21ed6024fa98a12df7b20a9159470c9a5330094e6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164180"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.roleManagement().directory().roleAssignments("lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1")
    .buildRequest()
    .delete();

```