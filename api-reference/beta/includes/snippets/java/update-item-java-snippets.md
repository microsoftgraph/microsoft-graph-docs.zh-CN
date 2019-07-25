---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5716373ea8454b41e1f9a23fd11201456b47db62
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860884"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = new DriveItem();
driveItem.name = "new-file-name.docx";

graphClient.me().drive().items("{item-id}")
    .buildRequest()
    .patch(driveItem);

```