---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f65227778bda41a3260c317c1baefaf6f53ffbdb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50984349"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.drive().bundles("{bundle-id}").children("{item-id}")
    .buildRequest()
    .delete();

```