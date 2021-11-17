---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6ce803a15eb0a3230df20a8da5d52de744a8d7dbe63d9c846e6c63deab33ab6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277386"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UsageRightCollectionPage usageRights = graphClient.users("{userId}").usageRights()
    .buildRequest()
    .filter("state in ('active', 'suspended') and serviceIdentifier in ('ABCD')")
    .get();

```