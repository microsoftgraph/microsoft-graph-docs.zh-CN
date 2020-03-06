---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3eea4f49b7984de9952ce1ff5d5576c06a0ebe8
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638004"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage transitiveMemberOf = graphClient.me().transitiveMemberOf()
    .buildRequest()
    .get();

```