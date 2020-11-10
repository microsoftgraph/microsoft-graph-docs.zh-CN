---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d6c608256728f4ff2cf80020638e0ed0c5f7710
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961938"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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