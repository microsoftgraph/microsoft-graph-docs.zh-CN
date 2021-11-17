---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3eb18f93ab8e5ad6c513ae945a3754bfdaad23f8de54c4b274af2cc6d337f188
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106664"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DataSource dataSource = graphClient.compliance().ediscovery().cases("5b840b94-f821-4c4a-8cad-3a90062bf51a").noncustodialDataSources("8e402dd7f3c94a3abc086e5d07db1c6d").dataSource()
    .buildRequest()
    .get();

```