---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6bd163ac4718b015272a9e9f9ffc6f36f05082d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59038270"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.sites("{siteId}").contentTypes("{contentTypeId}")
    .publish()
    .buildRequest()
    .post();

```