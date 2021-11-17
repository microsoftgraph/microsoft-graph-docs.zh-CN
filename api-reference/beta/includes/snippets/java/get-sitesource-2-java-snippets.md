---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81291e6414ebc03f1420d2d640aa45c3270c4dec14c5cb552f59c2881ed7bd0b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163151"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SiteSource siteSource = graphClient.compliance().ediscovery().cases("4c8f8f70-7785-4bd4-b296-c98376a2c5e1").custodians("2192ca408ea2410eba3bec8ae873be6b").siteSources("38304445-3741-3333-4233-344238454333")
    .buildRequest()
    .get();

```