---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e19acc8c9d33310d525ee122bc639c371ca5372e3fcce6462ffdb49ea8f86a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278722"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExtensionProperty extensionProperty = new ExtensionProperty();
extensionProperty.name = "extensionName";
extensionProperty.dataType = "string";
LinkedList<String> targetObjectsList = new LinkedList<String>();
targetObjectsList.add("Application");
extensionProperty.targetObjects = targetObjectsList;

graphClient.applications("{id}").extensionProperties()
    .buildRequest()
    .post(extensionProperty);

```