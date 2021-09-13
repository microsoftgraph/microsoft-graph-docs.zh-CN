---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 415784216fa7018c1879301c019a4b356f867ae82cc9aea1fba592497da1e1d1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162999"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveCollectionPage drives = graphClient.sites("{siteId}").drives()
    .buildRequest()
    .get();

```