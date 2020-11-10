---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09ae3e1b99dd791b78de74cdb63ddd33d0a5f8a4
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953871"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IProfilePhotoCollectionPage photos = graphClient.groups("{id}").photos()
    .buildRequest()
    .get();

```