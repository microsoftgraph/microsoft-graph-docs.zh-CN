---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 438e6f96c127234510f4d7224e4b85789a16efa2d38af0c29275777ddf149bd0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105820"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = new DriveItem();
driveItem.name = "Shared legal agreements";

graphClient.drive().items("{bundle-id}")
    .buildRequest()
    .patch(driveItem);

```