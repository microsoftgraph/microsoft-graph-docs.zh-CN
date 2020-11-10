---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35d129d2d7f647f32e740e0b2f6847867e6fffa0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964278"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemCollectionPage children = graphClient.drives("{drive-id}").items("{item-id}").children()
    .buildRequest()
    .get();

```