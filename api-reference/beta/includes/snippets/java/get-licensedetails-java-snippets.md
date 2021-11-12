---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ef25cf77ecc867af1453508562cb2c7ddcc95a6fe37a08abffb9d83ab9510ad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221492"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LicenseDetailsCollectionPage licenseDetails = graphClient.me().licenseDetails()
    .buildRequest()
    .get();

```