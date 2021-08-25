---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64318b2767d69454aec94e9695572c11434a1cce
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514393"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectorySetting directorySetting = graphClient.settings("f0b2d6f5-097d-4177-91af-a24e530b53cc")
    .buildRequest()
    .get();

```