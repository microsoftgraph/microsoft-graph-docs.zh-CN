---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf8a1662d60bb01fc8869cb7b1fe97cfdd12448f
ms.sourcegitcommit: ddeee0eec277df06d9e635e5b5c257d14c856273
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2021
ms.locfileid: "60783038"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContentTypeCollectionPage contentTypes = graphClient.sites("{site-id}").lists("{list-id}").contentTypes()
    .buildRequest()
    .get();

```