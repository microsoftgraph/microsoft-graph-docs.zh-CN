---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e134800ffbca92241fc0400c434024e984c3dad9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963079"
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