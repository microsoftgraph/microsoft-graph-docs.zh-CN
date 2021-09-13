---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0d372fa9a6e53f5b5667c9f65f25717ece9ac6dbed396dbe66752c85ad4cae7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278295"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{userId}").profile().addresses("{id}")
    .buildRequest()
    .delete();

```