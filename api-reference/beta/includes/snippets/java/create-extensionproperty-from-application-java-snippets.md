---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30666ccf2d3af2e4c84cae4ebff4153f23629e31
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973484"
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