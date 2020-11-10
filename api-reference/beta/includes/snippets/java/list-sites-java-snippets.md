---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6c6212486924ec7ad09315b2382ba061fa42325
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969714"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISiteCollectionPage sites = graphClient.sites()
    .buildRequest()
    .filter("siteCollection/root ne null")
    .select("siteCollection,webUrl")
    .get();

```