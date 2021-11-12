---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d8a0aea771ebf32607317f271ecdec1666d4a20b267162375e04b642d31a132
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328787"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "alexd@contoso.com";

graphClient.groups("{id}").acceptedSenders().references()
    .buildRequest()
    .post(directoryObject);

```