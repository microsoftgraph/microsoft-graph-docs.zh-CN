---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5261b5a05eba6098e01ccf263848bc67f5b017b5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893102"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> idsList = new LinkedList<String>();
idsList.add("84b80893874940a3-97b7-68513b600544");
idsList.add("5d6059b6368d-45f8-91e18e07d485f1d0");

LinkedList<String> typesList = new LinkedList<String>();
typesList.add("user");

graphClient.directoryObjects()
    .getByIds(idsList,typesList)
    .buildRequest()
    .post();

```