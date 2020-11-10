---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 458884f4a36a18cd083aeda550e4ccb2f133d696
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964046"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemCollectionPage children = graphClient.me().drive().special("{name}").children()
    .buildRequest()
    .get();

```