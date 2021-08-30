---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e9f3847177eafdb131f383f29f306a25ed6375fd7d3fe0de83e2d34a51da509
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162438"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ResourceSpecificPermissionGrantCollectionPage permissionGrants = graphClient.teams("14c981a4-dca9-4565-bae6-e13ada8861be").permissionGrants()
    .buildRequest()
    .get();

```