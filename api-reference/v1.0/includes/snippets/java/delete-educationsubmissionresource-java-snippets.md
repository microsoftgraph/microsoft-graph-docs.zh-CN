---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca24c833e83339b7273233e64c8fb5e56c11119c
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52990780"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("acdefc6b-2dc6-4e71-b1e9-6d9810ab1793").assignments("ad8afb28-c138-4ad7-b7f5-a6986c2655a8").submissions("fbe51c90-78b7-418a-b5f3-871bf8d8d21e").resources("f2387c3b-ec39-4bf2-a399-d7242677f024")
    .buildRequest()
    .delete();

```