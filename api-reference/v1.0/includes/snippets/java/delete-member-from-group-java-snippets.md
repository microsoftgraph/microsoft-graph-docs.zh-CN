---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb6b92ba3bf367bfbb60a62df73efbc04910c9d0
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48462643"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{group-id}").members("{directory-object-id}").reference()
    .buildRequest()
    .delete();

```