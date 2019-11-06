---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 046e35a107223d4a1076a3612fe01c0a81bbb933
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998937"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.Id = "{id}";

graphClient.applications("{id}").owners().references()
    .buildRequest()
    .post(directoryObject);

```