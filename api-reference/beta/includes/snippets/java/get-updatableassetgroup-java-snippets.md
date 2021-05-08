---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 951ff1b10e5a7687fa68f5ffe72669597bdbb8c3
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52238938"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UpdatableAsset updatableAsset = graphClient.admin().windows().updates().updatableAssets("5c55730b-730b-5c55-0b73-555c0b73555c")
    .buildRequest()
    .get();

```