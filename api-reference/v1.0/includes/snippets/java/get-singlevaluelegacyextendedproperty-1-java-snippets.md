---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c03c3e16ae924f58110ca6a6d995a04070593277c76278290b4510d622509ab8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279514"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = graphClient.me().messages("AAMkAGE1M2_bs88AACHsLqWAAA=")
    .buildRequest()
    .expand("singleValueExtendedProperties($filter=id%20eq%20'String%20%7B66f5a359-4659-4830-9070-00047ec6ac6e%7D%20Name%20Color')")
    .get();

```