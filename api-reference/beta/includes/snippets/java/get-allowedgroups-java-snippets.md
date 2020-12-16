---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4d626d711fe5d5017ae03dd8ad01388233898f4
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692723"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IGroupCollectionWithReferencesPage allowedGroups = graphClient.print().shares("{id}").allowedGroups()
    .buildRequest()
    .get();

```