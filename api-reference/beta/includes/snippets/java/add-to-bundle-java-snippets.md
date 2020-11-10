---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68e7354e5cf64725b251068a5a9e15d019bb471c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960283"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = new DriveItem();
driveItem.id = "123456!87";

graphClient.drive().bundles("{bundle-id}").children()
    .buildRequest()
    .post(driveItem);

```