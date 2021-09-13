---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0d5b746497067895bf5595f01e60543f2679b53b34fa5af36f51db1ce50108f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332814"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.communications().calls("2e1a0b00-2db4-4022-9570-243709c565ab")
    .keepAlive()
    .buildRequest()
    .post();

```