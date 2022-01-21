---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 921dbf87b9ad1a0ef9d7b97d75be4537a311bb6c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62093165"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BaseTaskListCollectionPage lists = graphClient.me().tasks().lists()
    .buildRequest()
    .get();

```