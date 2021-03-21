---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1fb5f45ccb220cfd5bb62e68fe5d473228ef7fe
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979345"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PermissionCollectionPage permissions = graphClient.me().drive().items("{item-id}").permissions()
    .buildRequest()
    .get();

```