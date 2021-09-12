---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d880787ba20962215e4b8f4ef46ee998ba4919d1e99a42fbae589f08eaaa1dfc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378808"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{id}";

graphClient.applications("{id}").owners().references()
    .buildRequest()
    .post(directoryObject);

```