---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b323ebbc55e54b5497678bd5135e032364ea1a47
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892597"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{user-id}")
    .buildRequest()
    .delete();

```