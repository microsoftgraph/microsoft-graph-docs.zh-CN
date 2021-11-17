---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e28d17087962649c9f4bd85cdcc945c62d81a85820c9e081fd7baaf4ee9f1639
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409459"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = graphClient.users("{id|userPrincipalName}").manager()
    .buildRequest()
    .get();

```