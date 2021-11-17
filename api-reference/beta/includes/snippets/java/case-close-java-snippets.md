---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b9f648a933614951737aa818c55a889cf2f02a04687912836fc2c00c83afd1b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163439"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.compliance().ediscovery().cases("061b9a92-8926-4bd9-b41d-abf35edc7583")
    .close()
    .buildRequest()
    .post();

```