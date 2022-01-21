---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7db32783ac035ffb26cd1f8257bcacf7d550437c112cc2c823a46d4f7ce8a0d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218870"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SynchronizationSchemaFunctionsCollectionPage functions = graphClient.servicePrincipals("{id}").synchronization().jobs("{jobId}").schema()
    .functions()
    .buildRequest()
    .get();

```