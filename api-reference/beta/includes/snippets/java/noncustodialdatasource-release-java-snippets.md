---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94cfe56115b2e5e20db6aef6d99c0ea9e57a9bf59a5adfd837b140904cb9a03a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161565"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.compliance().ediscovery().cases("5b840b94-f821-4c4a-8cad-3a90062bf51a").noncustodialDataSources("8e402dd7f3c94a3abc086e5d07db1c6d")
    .release()
    .buildRequest()
    .post();

```