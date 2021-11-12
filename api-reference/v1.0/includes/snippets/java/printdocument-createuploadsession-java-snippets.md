---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c312988564b58b83fef4d6c7a05c06adbd099befd77f7cc80e7d73548ede5c34
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158423"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintDocumentUploadProperties properties = new PrintDocumentUploadProperties();
properties.documentName = "TestFile.pdf";
properties.contentType = "application/pdf";
properties.size = 4533322L;

graphClient.print().printers("{printerId}").jobs("{printJobId}").documents("{printDocumentId}")
    .createUploadSession(PrintDocumentCreateUploadSessionParameterSet
        .newBuilder()
        .withProperties(properties)
        .build())
    .buildRequest()
    .post();

```