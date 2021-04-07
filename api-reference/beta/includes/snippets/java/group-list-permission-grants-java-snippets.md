---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5df4b986513954810962a11b4949f50d519ea67f
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611361"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ResourceSpecificPermissionGrantCollectionPage permissionGrants = graphClient.groups("14c981a4-dca9-4565-bae6-e13ada8861be").permissionGrants()
    .buildRequest()
    .get();

```