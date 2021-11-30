---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff094bf5b4172100e10e3b8a181c82f874dc7cd2
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61223533"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AttributeSet attributeSet = new AttributeSet();
attributeSet.description = "Attributes for engineering team";
attributeSet.maxAttributesPerSet = 20;

graphClient.directory().attributeSets("Engineering")
    .buildRequest()
    .patch(attributeSet);

```