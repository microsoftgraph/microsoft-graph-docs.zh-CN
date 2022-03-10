---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b604df193c670d9e10cbc7869a8d4894fad7ef2
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412476"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExtensionProperty extensionProperty = new ExtensionProperty();
extensionProperty.name = "jobGroup";
extensionProperty.dataType = "String";
LinkedList<String> targetObjectsList = new LinkedList<String>();
targetObjectsList.add("User");
extensionProperty.targetObjects = targetObjectsList;

graphClient.applications("fd918e4b-c821-4efb-b50a-5eddd23afc6f").extensionProperties()
    .buildRequest()
    .post(extensionProperty);

```