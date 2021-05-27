---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf8a1662d60bb01fc8869cb7b1fe97cfdd12448f
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52668719"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContentTypeCollectionPage contentTypes = graphClient.sites("{site-id}").lists("{list-id}").contentTypes()
    .buildRequest()
    .get();

```