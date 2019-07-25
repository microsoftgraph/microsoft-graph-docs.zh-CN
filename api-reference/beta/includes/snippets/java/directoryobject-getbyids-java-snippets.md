---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e134800ffbca92241fc0400c434024e984c3dad9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862398"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> idsList = new LinkedList<String>();
idsList.add("84b80893-8749-40a3-97b7-68513b600544");
idsList.add("5d6059b6-368d-45f8-91e1-8e07d485f1d0");

LinkedList<String> typesList = new LinkedList<String>();
typesList.add("user");

graphClient.directoryObjects()
    .getByIds(idsList,typesList)
    .buildRequest()
    .post();

```