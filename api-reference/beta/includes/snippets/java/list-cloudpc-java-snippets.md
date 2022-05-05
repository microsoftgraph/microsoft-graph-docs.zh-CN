---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 73593fd9b29cd43c8f4449d01269b8ed9765a74d
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211972"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPCCollectionPage cloudPCs = graphClient.me().cloudPCs()
    .buildRequest()
    .get();

```