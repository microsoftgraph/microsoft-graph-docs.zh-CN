---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3abd562ae4c11e861f60e694c1629c409cbfc9ff
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044884"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContentType contentType = new ContentType();
contentType.name = "docSet";
contentType.description = "custom docset";
ContentType base = new ContentType();
base.name = "Document Set";
base.id = "0x0120D520";
contentType.base = base;
contentType.group = "Document Set Content Types";

graphClient.sites("{id}").contentTypes()
    .buildRequest()
    .post(contentType);

```