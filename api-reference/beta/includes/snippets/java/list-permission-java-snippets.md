---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 680bd9072fb751bd1a42ce1b65edbe88e892aaebc54467b3751be4e369faf50c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903932"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PermissionCollectionPage permissions = graphClient.sites("{sitesId}").permissions()
    .buildRequest()
    .get();

```