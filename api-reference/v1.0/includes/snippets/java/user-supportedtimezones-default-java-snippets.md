---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55cd81dc7f68307a867cdfa4a025fa26221989e1d283c78ca74888dabeb18bb8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220553"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookUserSupportedTimeZonesCollectionPage supportedTimeZones = graphClient.me().outlook()
    .supportedTimeZones()
    .buildRequest()
    .get();

```