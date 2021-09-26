---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f94e5ef1792b7446b64692163a9a98154928f4fb5a39eac46265aa3aad1cf1e6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158310"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.deviceManagement().virtualEndpoint().onPremisesConnections("{id}")
    .buildRequest()
    .delete();

```