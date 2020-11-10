---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d8d058d8dde653af6c979aac4a40cbf6d0ec6a2
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955835"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveCollectionPage drives = graphClient.me().drives()
    .buildRequest()
    .get();

```