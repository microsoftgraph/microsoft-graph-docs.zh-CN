---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 358c38ae0d457c35ca550a85fc4f19318891eba5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971467"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("{class-id}")
    .buildRequest()
    .delete();

```