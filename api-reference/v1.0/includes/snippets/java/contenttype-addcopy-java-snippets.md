---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fef396a56e730cf39fd4619c5befbbe69df056c7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147702"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String contentType = "https://graph.microsoft.com/v1.0/sites/{site-id}/contentTypes/0x0101";

graphClient.sites("{site-id}").lists("{list-id}").contentTypes()
    .addCopy(ContentTypeAddCopyParameterSet
        .newBuilder()
        .withContentType(contentType)
        .build())
    .buildRequest()
    .post();

```