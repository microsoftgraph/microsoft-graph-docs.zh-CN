---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5fefef2b3b61afe19893fdbafc4f87a630445eb626154ac66dd215d648792eab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105629"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ResourceSpecificPermissionGrantCollectionPage permissionGrants = graphClient.groups("14c981a4-dca9-4565-bae6-e13ada8861be").permissionGrants()
    .buildRequest()
    .get();

```