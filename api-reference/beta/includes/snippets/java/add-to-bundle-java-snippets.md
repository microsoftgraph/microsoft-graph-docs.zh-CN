---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed18022ec3a1e897368bd3a5712281579ead07148bb87ce3f21bcffc840cc2a5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105272"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = new DriveItem();
driveItem.id = "123456!87";

graphClient.drive().bundles("{bundle-id}").children()
    .buildRequest()
    .post(driveItem);

```