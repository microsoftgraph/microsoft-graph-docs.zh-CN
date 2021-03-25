---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ee2de2f4dc354ec14d03d588265142c7b9213ff
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208119"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Call call = graphClient.communications().calls("2f1a1100-b174-40a0-aba7-0b405e01ed92")
    .buildRequest()
    .get();

```