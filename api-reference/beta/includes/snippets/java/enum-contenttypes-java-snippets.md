---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6ff82d40fd8390d76179ab0b3040f5314914ba0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965057"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContentTypeCollectionPage contentTypes = graphClient.sites("{site-id}").contentTypes()
    .buildRequest()
    .get();

```