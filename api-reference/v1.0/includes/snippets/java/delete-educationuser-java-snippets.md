---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3bc133a03d029a4d5bbcd0fb269ed05d4f33e2be514d6d21e8bbf8becc0bb84a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221425"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().users("{user-id}")
    .buildRequest()
    .delete();

```