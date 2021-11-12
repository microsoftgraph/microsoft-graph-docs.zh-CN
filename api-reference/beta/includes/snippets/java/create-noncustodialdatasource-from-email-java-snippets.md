---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7cbc133c3abfe2e7362e0b9381bb96e792c87a12
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "60927042"
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