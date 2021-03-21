---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02312d4b90fad2d7ce7a31f4b96c61118140974d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974491"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Domain domain = graphClient.domains("contoso.com")
    .buildRequest()
    .get();

```