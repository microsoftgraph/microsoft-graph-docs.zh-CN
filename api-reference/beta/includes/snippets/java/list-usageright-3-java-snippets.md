---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a5512bbaaa82e9edb5b2dcd922c91619de5fdd991c976fa69bdf78bbbfe5ef7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219830"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UsageRightCollectionPage usageRights = graphClient.users("{userId}").usageRights()
    .buildRequest()
    .get();

```