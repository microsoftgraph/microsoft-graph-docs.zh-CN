---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9494e7c479e23265962c3b1bd433857668cd5f8a915999865a4cdb57598729c6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333354"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Permission permission = graphClient.me().drive().items("{item-id}").permissions("{perm-id}")
    .buildRequest()
    .get();

```