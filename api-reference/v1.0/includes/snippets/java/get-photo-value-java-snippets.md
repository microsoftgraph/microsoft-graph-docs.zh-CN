---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95316f53307ec0c9014859f7771e3d3527919698
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428805"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Stream stream = graphClient.users("{id|userPrincipalName}").photo().content()
    .buildRequest()
    .get();

```