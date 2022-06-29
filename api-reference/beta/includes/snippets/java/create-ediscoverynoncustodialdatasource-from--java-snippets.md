---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 260aa6cc8b5016fad45040f5d5243a2b5ff4a14e
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66502826"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoveryNoncustodialDataSource ediscoveryNoncustodialDataSource = new EdiscoveryNoncustodialDataSource();
ediscoveryNoncustodialDataSource.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/noncustodialDataSources/39333641443238353535383731453339"));

graphClient.security().cases().ediscoveryCases("b0073e4e-4184-41c6-9eb7-8c8cc3e2288b").searches("c61a5860-d634-4d14-aea7-d82b6f4eb7af").noncustodialSources().references()
    .buildRequest()
    .post(ediscoveryNoncustodialDataSource);

```