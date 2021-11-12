---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6c6d11d9e8da721c0abca1a9bcbffd331cb02f3ae7d2968b1374fef65a0cf5d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218917"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookCategory outlookCategory = graphClient.me().outlook().masterCategories("de912e4d-c790-4da9-949c-ccd933aaa0f7")
    .buildRequest()
    .get();

```