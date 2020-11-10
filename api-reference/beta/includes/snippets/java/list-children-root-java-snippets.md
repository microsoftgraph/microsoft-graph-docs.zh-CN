---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 77b692f0932c9bd3b00cbbcd6ac0ec1691664b68
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964277"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemCollectionPage children = graphClient.me().drive().root().children()
    .buildRequest()
    .get();

```