---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cebcf09f2cd22af2e724fc80abb67f28835f8db2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983853"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String storageLocation = "storageLocation-value";

graphClient.users("{id}")
    .exportPersonalData(UserExportPersonalDataParameterSet
        .newBuilder()
        .withStorageLocation(storageLocation)
        .build())
    .buildRequest()
    .post();

```