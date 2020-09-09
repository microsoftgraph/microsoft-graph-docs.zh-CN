---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aed02abad2e45568dee82380adbec8de142d0a27
ms.sourcegitcommit: 01f73b4dce6f885da18d62fe800b387c286c7a8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/09/2020
ms.locfileid: "47413325"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.Id = "{id}";

graphClient.groups("{group-id}").members().references()
    .buildRequest()
    .post(directoryObject);

```