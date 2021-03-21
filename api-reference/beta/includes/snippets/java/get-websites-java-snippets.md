---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83f9a2f912b240c2e667a9c59a953e977f095375
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980823"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonWebsiteCollectionPage websites = graphClient.me().profile().websites()
    .buildRequest()
    .get();

```