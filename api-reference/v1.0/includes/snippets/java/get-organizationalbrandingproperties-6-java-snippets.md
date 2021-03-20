---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82dc178e19931c6a66ebc318cd1c3e4d1fa93bb1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949503"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Accept-Language", "de"));

InputStream stream = graphClient.customRequest("/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo", InputStream.class)
    .buildRequest( requestOptions )
    .get();

```