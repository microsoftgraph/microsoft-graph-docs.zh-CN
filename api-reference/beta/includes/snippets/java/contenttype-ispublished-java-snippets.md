---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2bada94d0d56d7f9b07a9d8b16f4631886575159b2f612d756d4a9facbd4ebdb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220908"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean _boolean = graphClient.sites("{siteId}").contentTypes("{contentTypeId}")
    .isPublished()
    .buildRequest()
    .get();

```