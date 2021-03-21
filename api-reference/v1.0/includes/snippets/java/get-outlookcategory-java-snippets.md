---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9c481cd0a112f829d581411d36a1f1babdeb2a7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968227"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookCategory outlookCategory = graphClient.me().outlook().masterCategories("de912e4d-c790-4da9-949c-ccd933aaa0f7")
    .buildRequest()
    .get();

```