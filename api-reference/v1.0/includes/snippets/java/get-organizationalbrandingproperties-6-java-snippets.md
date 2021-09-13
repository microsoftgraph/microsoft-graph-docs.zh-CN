---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f72b6b18f59055b14056e9b9dce5398ddb825ccd8a54e5ecd96e9ef1d43fd187
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162026"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Accept-Language", "de"));

InputStream stream = graphClient.customRequest("/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo", InputStream.class)
    .buildRequest( requestOptions )
    .get();

```