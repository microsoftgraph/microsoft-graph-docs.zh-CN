---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7cbc133c3abfe2e7362e0b9381bb96e792c87a12
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52266909"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

NoncustodialDataSource noncustodialDataSource = new NoncustodialDataSource();
noncustodialDataSource.applyHoldToSource = true;
UserSource dataSource = new UserSource();
dataSource.email = "adelev@contoso.com";
noncustodialDataSource.dataSource = dataSource;

graphClient.compliance().ediscovery().cases("5b840b94-f821-4c4a-8cad-3a90062bf51a").noncustodialDataSources()
    .buildRequest()
    .post(noncustodialDataSource);

```