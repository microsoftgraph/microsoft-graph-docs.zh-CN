---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64ead35ca48d9f9e3f093db1d8509d21efda2c8045cf07af2f4f348c7477f78e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105181"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Drive drive = graphClient.groups("{groupId}").drive()
    .buildRequest()
    .get();

```