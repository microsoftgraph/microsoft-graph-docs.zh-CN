---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70e3432ac41a9b9c216793f243a064a6c82ce6080d6f15a4c6b44f654e3cf1ca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220524"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{id}";

graphClient.devices("{id}").registeredUsers().references()
    .buildRequest()
    .post(directoryObject);

```