---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d81e0bac28c09f19c5155627e6a8e47fb2ddeed
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226508"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AttributeSet attributeSet = new AttributeSet();
attributeSet.id = "Engineering";
attributeSet.description = "Attributes for engineering team";
attributeSet.maxAttributesPerSet = 25;

graphClient.directory().attributeSets()
    .buildRequest()
    .post(attributeSet);

```