---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21e1f10893e1b3f010782604232ba93aa138a256
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204285"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserCollectionPage users = graphClient.users()
    .buildRequest()
    .select("ext55gb1l09_msLearnCourses")
    .get();

```