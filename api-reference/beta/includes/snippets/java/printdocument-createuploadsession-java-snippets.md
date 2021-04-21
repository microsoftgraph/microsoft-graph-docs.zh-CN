---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2035c43cddc9c8bce72ed034a64e2a8219daecc9
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921850"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintDocumentUploadProperties properties = new PrintDocumentUploadProperties();
properties.documentName = "TestFile.pdf";
properties.contentType = "application/pdf";
properties.size = 4533322L;

graphClient.print().shares("1c879027-5120-4aaf-954a-ebfd509a3bcc").jobs("46207").documents("9001bcd9-e36a-4f51-bfc6-140c3ad7f9f7")
    .createUploadSession(PrintDocumentCreateUploadSessionParameterSet
        .newBuilder()
        .withProperties(properties)
        .build())
    .buildRequest()
    .post();

```