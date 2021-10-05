---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a39b3d2d87decd5e37fb4f4e9b3046c1b6675d6bf51b399e0ec3bcc1d0d5e7aa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332032"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.subscriptions("7f105c7d-2dc5-4530-97cd-4e7ae6534c07")
    .buildRequest()
    .delete();

```