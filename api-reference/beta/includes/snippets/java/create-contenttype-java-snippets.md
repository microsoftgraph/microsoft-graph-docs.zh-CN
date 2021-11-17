---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ec2fa43507c95b6f81fa798e609236fd056b188e5c2133b02ee2e6c5bc90a01
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163068"
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