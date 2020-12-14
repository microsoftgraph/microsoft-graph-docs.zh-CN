---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c4de91ad2d14e33f17b93594ba38ed27b15fe322
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658808"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SiteSource siteSource = graphClient.compliance().ediscovery().cases("4c8f8f70-7785-4bd4-b296-c98376a2c5e1").custodians("2192ca408ea2410eba3bec8ae873be6b").siteSources("38304445-3741-3333-4233-344238454333")
    .buildRequest()
    .get();

```