---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 705cba4f36d46d741d90c36321aa3cdef095893b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771580"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IGroupCollectionWithReferencesPage allowedGroups = graphClient.print().shares("{printerShareId}").allowedGroups()
    .buildRequest()
    .get();

```