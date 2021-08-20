---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dadf1ae9f8e1c2fed0d82834621566f1d952178b4f695d77586c7ac4853f0255
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163273"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{id}";

graphClient.groups("{group-id}").members().references()
    .buildRequest()
    .post(directoryObject);

```