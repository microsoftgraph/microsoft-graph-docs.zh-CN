---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ddd500ac7477940fa24112caa1d39dec2a7579ba6489cae6e6c24075b6e8a18d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220214"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{id}";

graphClient.servicePrincipals("{id}").owners().references()
    .buildRequest()
    .post(directoryObject);

```