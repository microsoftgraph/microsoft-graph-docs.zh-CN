---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0fd7c711794e1ba8c1e929d8ccbbcec3db066df05be6250c9f7315e1b08df0c2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164088"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{userId}").profile().notes("{id}")
    .buildRequest()
    .delete();

```