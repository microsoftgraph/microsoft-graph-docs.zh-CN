---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c85a7e165e107c8407f033ed00d49aca605f5cc1960ce47cb0b433020b5888f6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279552"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserAccountInformation userAccountInformation = graphClient.me().profile().account("{id}")
    .buildRequest()
    .get();

```