---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 638aa02282eed0490f8bfff2706fc95576faeab2
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241446"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.admin().windows().updates().updatableAssets("{azureADDeviceId}")
    .buildRequest()
    .delete();

```