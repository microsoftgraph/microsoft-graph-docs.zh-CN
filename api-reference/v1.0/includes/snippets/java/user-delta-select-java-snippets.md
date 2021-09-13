---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4657f47039a496c29f87b431a743950330c9d7426db1f620de57014f0c9da5ba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105296"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserDeltaCollectionPage delta = graphClient.users()
    .delta()
    .buildRequest()
    .select("displayName,jobTitle,mobilePhone")
    .get();

```