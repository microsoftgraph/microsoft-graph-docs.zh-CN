---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b7324c2135655a4a9dfd86eb40bf36c620e794a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978939"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.organization("{id}").certificateBasedAuthConfiguration("{id}")
    .buildRequest()
    .delete();

```